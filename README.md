# Welcome to the Online Companion for Network Science in Archaeology

To visit the rendered bookdown version of this project [click here](https://book.archnetworks.net)

[![Docker Image CI](https://github.com/mpeeples2008/ArchNetSci/actions/workflows/docker-image.yml/badge.svg)](https://github.com/mpeeples2008/ArchNetSci/actions/workflows/docker-image.yml)

This project serves as a companion to the Cambridge Manuals in Archaeology book *Network Science in Archaeology* by Tom Brughmans and Matthew A. Peeples (2023). This document contains a series of tutorials that outline methods for managing, analyzing, and visualizing network data, primarily using the R programming language. We provide code and examples to replicate the analyses presented in the book as well as many other useful tools. The bulk of this Online Companion is designed to be used with the book in hand to expand on topics covered in the published version. Part I of this document (see the Table of Contents) is focused on helping you get started in R and R-Studio. Part II which includes sections 2 through 7 corresponds to the topics and information covered in Chapters 2 through 7 of the Brughmans and Peeples book. Part III (Going Beyond the Book) includes tutorials beyond the scope of the published book including "advanced" topics that require additional detailed description and knowledge of the methods presented in Parts I and II. We plan to continue to add to and expand Part III in the future. You can use the table of contents on the left-hand side of your screen to jump directly to a particular section and the table and contents on the right to navigate within each section. We have also created a quick TOC reference if you are seeking something in particular. 


For more information on the book and the authors check out the project website here: [archnetworks.net](https://archnetworks.net).

**Cite this document as:**

> Peeples, Matthew A. and Tom Brughmans (2023). *Online Companion to Network Science in Archaeology*. <https://archnetworks.net>, Accessed 21 March 2023.

**The associated book can be cited as**

> Brughmans, Tom and Matthew A. Peeples (2023). *Network Science in Archaeology.* Cambridge Manuals in Archaeology. Cambridge University Press, Cambridge, UK.

## How Should I Use This Online Companion?

Check the bookdown [Online Companion](https://book.archnetworks.net) to get started.

The tutorials here are designed to complement the text of the associated book (Brughmans and Peeples 2023) but can also stand alone as a guide to implementation of network analyses in R if you have a basic background in network methods and terminology. Although each section of this guide builds upon the previous sections in terms of network concepts and R methods, the sections are each independent in terms of data, examples, and code and can be run out of order if you choose.

A few suggestions on where to start:

* If you are new to network analysis and R, we would suggest going through each section of this document, starting with Part I: Getting Started with R and then going through Part II in order as you following along with the corresponding chapters in the book.
* If you are already familiar with R but new to network analysis, you can start with Section 2 in Part II to set up your data and work space, and then follow along with the remaining numbered sections and associated book chapters as you read.
* If you are already a network analyst and confident R user and are just looking for code chunks to implement something in particular, feel free to skip around. We have tried to make each section as independent as possible so that you can pick and choose what you want to work on. Use the Table of Contents to find topics quickly.
* If you're a real pro and are designing your own network analyses or visualizations, we would love it if you contributed to the project to help this document grow.

## Reproducibility

The most recent version of this document was built with R 4.2.2 and Python 3.8. We suggest you use a recent version of R (>= 4.2) and Python (>= 3.8) when attempting to use the code in this document. 

The content of this document is meant to be as accessible and reproducible as possible. The source code used to produce this document along with all of the data used in analyses are available on [GitHub](https://github.com/mpeeples2008/ArchNetSci). This GitHub repository allows users to open issues, contribute to the document, or help fix typos or other errors (see information about contributing below). We have also opened a GitHub discussion board with this repository where users can ask questions about any data or code in the repository without making edits or issue requests directly. 

The easiest way to reproduce this document is to launch the project directly in your browser using [Binder](https://mybinder.org/). When you click on the link below it will open a browser based instance of R studio with all of the required packages and files. From there you can test and evaluate the code directly.

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/mpeeples2008/ArchNetSci/main)

You can also run the code and generate documents locally using R and R Studio. Download the entire R repository here: [main.zip](https://github.com/mpeeples2008/ArchNetSci/archive/refs/heads/main.zip). Unzip the files and then:

* Open the "ArchNetSci.Rproj" file in R studio.
* Use the `renv::restore()` command to install the required packages and dependencies. Note that this is a large document that uses many packages so this may take some time.
* You will then be able to browse the files and execute all of the code in the repository.

This online bookdown document has been deployed using the Netlify platform and the badge below shows the current status of the build hosted at [https://book.archnetworks.net](https://book.archnetworks.net).

[![Netlify Status](https://api.netlify.com/api/v1/badges/266d5736-f13a-4de4-b812-141c023f3a09/deploy-status)](https://app.netlify.com/sites/archnetworks/deploys)

## Computational Archaeology Discord Community

We have created an [Archaeological Network Science Channel on the Computational Archaeology Discord Server](https://discord.gg/Z9UXwjASM5), which we hope will provide an additional venue for archaeological network practitioners to collaborate, interact, and ask for help with this document or with archaeological networks (and other computational methods). We invite you to use this as a place to ask questions of the authors and the community at large. Note that this Discord is subject to the same [code of conduct](https://github.com/mpeeples2008/ArchNetSci/blob/main/CODE_OF_CONDUCT.md) we use for the GitHub repository and you must abide by that agreement to participate. We require that you have a Discord account with a verified email address.

[Join the Computational Archaeology Discord](https://discord.gg/Z9UXwjASM5)&nbsp; &nbsp;&nbsp; &nbsp;  ![](https://discordapp.com/api/guilds/975267909012189184/widget.png?style=shield)

## New to R and R Studio?

This tutorials in this document are built for users with a basic familiarity with R and R-studio. If you are a first time R user and need help getting R and R studio installed and up and running, we have created a detailed guild to [Getting started with R](https://book.archnetworks.net/gettingstarted#GettingStarted). This document covers the installation of the required software and provides a basic introduction to the R programming environment that we hope will be enough to get you started. 

If you already have a basic familiarity with R and want to go further, there are numerous additional resources (most are completely free) to help you learn. Some resources we would recommend include *R for Data Science* [(Wickham and Grolemund 2017)](https://r4ds.had.co.nz/), *Advanced R* [(Wickham 2019)](https://adv-r.hadley.nz/), *the R Cookbook, 2nd edition* [(Long and Teetor 2019)](https://rc2e.com/somebasics), and *R in Action* and the associated *Quick-R* website [(Kabacoff 2015)](https://www.statmethods.net/). In addition to this [Ben Marwick](https://anthropology.washington.edu/people/ben-marwick) has created an excellent repository of [resources for using R in archaeology](https://github.com/benmarwick/ctv-archaeology) as well as an ever-growing list of archaeological publications that include R code. The website associated with this book [archnetworks.net](https://www.archnetworks.net) also includes a list of archaeological articles focused on network research that include data and code. Reproducing published results is, in our experience, one of the best ways to learn advanced techniques and data management in R so we suggest you give it a try.

## Contribute To the Project

We welcome contributions to this project from the community and the GitHub platform helps us facilitate that. You will first need to [sign up for a GitHub account](https://github.com/) and log in. If you find something that needs updating or changing (typos or errors) you can simply click the "Edit source" link at the right sidebar on the relevant page and then click the edit icon found near the top of the code block and make your proposed changes. These changes will be saved in a new "fork" of the document and we will review these and implement them where relevant and happily add your name to our list of contributors. Note that we generally use the [tidyverse style guide](https://style.tidyverse.org/) for formatting code and comments.

If you detect a larger error such as code not running or if you would like to request a new feature or update, you can create an issue using the [issue tracker](https://github.com/mpeeples2008/ArchNetSci/issues) page associated with the project repository.

All contributors must agree to adhere to our [code of conduct](https://github.com/mpeeples2008/ArchNetSci/blob/main/CODE_OF_CONDUCT.md).

## Help Support this Project and Build the Community

We are devoted to seeing the community of archaeological network practitioners grow and we hope our book and these online resources will help to make this happen. You can support the growth of our community too!

* Spread the word to your friends and colleagues
* Share links to these online resources on social media using the [#archnetworks](https://twitter.com/search?q=%23archnetworks&src=typed_query) hashtag
* Please cite the book *and* the Online Companion if you use methods or code from this document. [Citation Info](https://github.com/mpeeples2008/ArchNetSci/blob/main/CITATION.bib)
* Star the [GitHub project repository](https://github.com/mpeeples2008/ArchNetSci) and contribute to the project
* [Join the Computational Archaeology Discord](https://discord.gg/Z9UXwjASM5) and invite other interested people
* Share articles, teaching resources, data, or other archaeological network materials for posting on our associated website [(archnetworks.net)](https://archnetworks.net)

## Project License

[![](https://i.creativecommons.org/l/by-nc-nd/4.0/88x31.png)](http://creativecommons.org/licenses/by-nc-nd/4.0/)

This Online Companion to Archaeological Network Science is licensed under a [Creative Commons Attribution-NonCommercial-NoDerivitives 4.0 International License](http://creativecommons.org/licenses/by-nc-nd/4.0/).

## Acknowledgements

This project and the associated book were made possible thanks to the support of several generous funding sources including: The Carlsberg Foundation, in the context of the Past Social Networks Project (CF21-0382); the National Science Foundation through both the Archaeology and the Measurement, Methodology, and Statistics programs (grant #1758690 and #1758606); and the School of Human Evolution and Social Change at Arizona State University. Thank you to Jens Emil Bødstrup Christoffersen for providing detailed comments on and for testing the initial version of this document. Any errors that remain are our own.
