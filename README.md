# IO Industrial Employee Handbook and Policy Manual

This repository contains the current employee handbook and
policies that employees are expected to abide by.

Requirements:
* Sphinx: http://sphinx-doc.org/contents.html
 * version 1.2.3 or later
* LaTeX (and pdflatex, and various LaTeX packages)
* Graphviz (in particular, "dot"): http://www.graphviz.org/

On Debian and Ubuntu:

>```
># apt-get install python-sphinx texlive texlive-latex-extra libalgorithm-diff-perl \
>                  texlive-humanities texlive-generic-recommended graphviz \
>                  texlive-generic-extra
>```
>
>If the version of python-sphinx installed is too old, then an additional
>new version can be installed with the Python package installer:
>
>```
>$ apt-get install python-pip
>$ pip install --user --upgrade Sphinx
>$ export SPHINXBUILD=~/.local/bin/sphinx-build
>```
>
>You will need latexdiff v1.2.1 or later to create the changebars PDF version
>of the document.
>Until distributions catch up with the latest release you will need to install
>it directly from the github repo.
>
>```
>$ git clone https://github.com/ftilmann/latexdiff
>$ export PATH=$PWD/latexdiff/:$PATH
>```
>
>Export SPHINXBUILD (see above) if Sphinx was installed with pip --user, then follow Make commands below

On Mac OS X:

> Install [MacTeX](http://tug.org/mactex/)
>
> Install pip if you do not have it:
>```
>$ sudo easy_install pip
>```
>Install Sphinx
>```
>pip install --user --upgrade Sphinx
>Or
>sudo pip install --upgrade Sphinx
>```
>
>If you are using [brew](http://brew.sh) then you can install graphviz like this:
>```
brew install graphviz
>```
>If you are using [macports](https://www.macports.org/) then you can install graphviz like this:
>```
>$ sudo port install graphviz
>```

Make commands:

>```
>$ make latexpdf # For generating pdf
>$ make html # For generating a hierarchy of html pages
>$ make singlehtml # For generating a single html page
>```

Output goes in ./build subdirectory.
