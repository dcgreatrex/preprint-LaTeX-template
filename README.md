# preprint-LaTeX-template

## Overview

A LaTeX template designed to make it easier to produce experimental report preprints prior to sending to journals such as J. Neurosci, PNAS, Frontiers, Cell, Trends Cogn. Sci [*] This template has been adapted from the standard open source PNAS LaTeX class template found [here](http://www.pnas.org/page/authors/latex).

The template copies preprint formats found on the following sites:
* [psyarxiv](https://psyarxiv.com)
* [biorxiv](https://www.biorxiv.org)

The template design is based on the following preprint papers:
[1](https://www.biorxiv.org/content/early/2018/01/12/247460)
[2](https://www.biorxiv.org/content/early/2018/02/19/268045)
[3](https://www.biorxiv.org/content/early/2017/12/15/234070)
[4](https://psyarxiv.com/svf6c/)

## Motivation
Recently, authors in the timing and decision making literatures are publishing experimental papers to either psyarxiv or biorxiv prior to them being accepted by journals listed [*].
They are using generic report structures that remain fixed across publication and presumably make it easier to transfer preprint content into target publication templates.
The motivation of this repository is to deliver a LaTeX template that 
a) copies their preprint style, and
b) makes it easier to structure report content prior to it being accepted by a journal.

## Quickstart
* Clone or download all content in this repository
* Install LaTeX on your machine. Follow instructions found [here](https://www.latex-project.org/get/).
* cd into the cloned respository and open the main tex file called 'preprintarticle.tex'. 
* In 'preprintarticle.tex' add title, author and affiliation information to the variables named:
  * title
  * author
  * affil
  * correspondingauthor
* Save report content in the corresponding .tex files saved in the subdirectory named 'content'. Content files currently available:
  * Abstract (abstract.tex)
  * Significance statement (significance.tex)
  * Introduction (introduction.tex)
  * Results (results.tex)
  * Discussion (discussion.tex)
  * Supporting information (supportinginfo.tex)
  * Methods (methods.tex)
  * Supplementary materials (supplementarymat.tex)
* Save report images in the subdirectory named 'images'.
* Add bibliographic information to the file called 'preprintarticle.bib'. 
Alternatively, use an alternative master .bib file that you have saved on your machine.
To do this replace [\bibliography{preprintarticle}] with [\bibliography{XXX}] (ignoring squared brackets) where XXX is the name of your master .bib file on line 48 of 'preprintarticle.tex'.
Ensure that your master .bib file is either saved in the project repository or somewhere on your start-up LaTeX search path.
* Generate the .pdf file by running 'make' on preprintarticle.tex. Alternately, open 'preprintarticle.tex' in a LaTeX editor such as [TeXworks](http://www.tug.org/texworks/), [TeXstudio](https://www.texstudio.org/), or similar, and press 'run'. 
After compilation, preprintarticle.pdf will appear in the project repository. 
