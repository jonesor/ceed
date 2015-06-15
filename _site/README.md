# CEED Workshop

This is code and text behind my (Owen Jones's) CEED Workshop site. The material is intended for a workshop called "The Era Of Big Data Hits Conservation" held on 15-19th June 2015 at the ARC Centre for Excellence in Environmental Decisions (CEED). The workshop covers lots of ground, and this is just a small part of it concerning the use of phylogenetic information in conservation.

The site is based on Hadley Wickham's site for his Advanced R Programming book.

The site is built using Jekyll, with a custom plugin to render `.rmd` files with
knitr and pandoc. To create the site, you need:

* jekyll and s3_websiter gems: `gem install jekyll s3_website`
* [pandoc](http://johnmacfarlane.net/pandoc/)
* [knitr](http://yihui.name/knitr/): `install.packages("knitr")`
* [bookdown](https://github.com/hadley/bookdown): 'install_github("hadley/bookdown")'
* [Ruby](https://www.ruby-lang.org/en/) - you probably already have this installed.

## .gitignore

Add the following to your `.gitignore` file.

`Temp.html`

`Temp.Rmd`

`*.Rproj`

`_site`

##Copying and deploying this site (e.g. to create a similar one)

I assume you are using a Mac with OSX.

* Create a new repository, `XXX`, with a `.gitignore` file
* Create a new branch of `XXX` called `gh-pages` (i.e. have two branches named "`master`" and "`gh-pages`")
* Use the Github app to clone `XXX` to your computer.
* Place the contents of `ceed` in the `XXX` directory master branch.
* Open Terminal, navigate to your `XXX` directory, run '`jekyll serve`' and watch as directory "`_site`" is created. It may take a few moments.
* Stop the jekyll server (ctrl-c)
* Move "`_site`" to the desktop.
* In GitGub app, switch to the `gh-pages` branch.
* Move the contents of "`_site`" to the `XXX` directory of the `gh-pages` branch.
* Commit and synchronise to GitGub.
* Your site should be visible at `http://username.github.io/XXX`
