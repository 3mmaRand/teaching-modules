# Forwards Package development modules

**A WORK IN PROGRESS!**

## Computing requirements
[Computing requirements overall](Computing_requirements.md)

## Modules

### Packages in a nutshell

What is a package - unit of sharable code    
Why write a package? impact, recognition, documentation   
Where do they live on your computer  
where do they come from  
Components of a package: demo of package we will develop; demo of well known  
Package states  
Forwards approach to packages: devtools and rstudio  
overview of development process; needs rtools/XCode/`r-base-dev`, git recommended   

Ref: Chapter 4 Package structure and state

#### Learning Objectives
At the end of this module the successful learner will be able to:  
* explain the rationale for wrting packages  
* find and explore their own package library/libraries  
* describe the different states a package can be in  
* describe the key components of a package  
* outline the development of a package using devtools   

#### Prerequisites
* r user, otherwise very few
* r and rstudio installed

---

### Setting up your system to develop version controlled package with `devtools` in RStudio

R version, Rstudio versions  - discuss but should have been done  
packages needed: devtools, roxygen2, testthat, knitr  - ditto  
R build toolchain: Rtools(windows) or XCode (mac) or `r-base-dev`; `has_devel() `   - ditto  
git - ditto - check Tools | Global Options | Git/SVN tab - path to git included

Opportunity to carry out in session if not done.  

we need devtools but development process includes restarting session therefore put this in .Rprofile
```
if (interactive()) {
  suppressMessages(require(devtools))
}
```
Can be done with `use_devtools()`  
Add `options()` to .Rprofile to set maintainer name, license defaults.  

Use of RStudio projects

set up for use of git and github in Rstudio - can do with a RS project (no need to be a pkg) - minimal/little detail on git (refer to a more detailed module on git)
usethis::use_git() - initilaises a git repo and makes initial commit (if you select that option)

Do Tools | Version Control | Project Setup and selcting git will also initialise a git repo

github: using "Existing project github last" and https approach - use_github(), error, browse_github_token(), generate and copy token, add to .Renviron with usethis::edit_r_environ(), restart and do use_github(),

Ref: Chapter 3 System setup; Chapter 2 The whole game 2.5 and 2.17 

#### Learning Objectives
At the end of this module the successful learner will be able to:  
* list and install the programs and packages required for version controlled package development with `devtools` in RStudio  
* check these are available to RStudio
* edit their .Rprofile to ensure devtools is loaded  
* configure git for use, initialise an RStudio project as a git repo
* authorise and link to a github repo  
*   

#### Prerequisites
* r and rstudio installed
* git installed
* github account
* Packages in a nutshell or equivalent - desirable but not essential

---

### A simple package

minimal package
load devtools  
describe pkg to be built; 
two approaches possible chose one or cover both??
1. Existing project, GitHub last: create_package, use_git, use_github or 2.
2. New project, GitHub first: create repo on gh, new project | version control | git.  then set up package structure with Tools > Project Options > Build Tools. Select Package and use_description(), use_namespace(), use_r("fnctname") 
make a function, load_all(), check(), add roxygen, document(), alter DESCRIPTION, add a LICENSE

Ref: Chapter 2 The whole game

#### Learning Objectives
At the end of this module the successful learner will be able to:  
* create a simple version controlled package  
* link the package to github  
* explain the key components of a minimal package  
* create and document a function with roxygen2 and document()
* use the package interactively with load_all()  
* use check() to execute R CMD check
* explain, create and populate a DESCRIPTION file
* add a LICENSE file and explain the rationale for doing so

#### Prerequisites
* r and rstudio installed
* git installed, github acc, github use authorised
* devtools, roxygen2, testthat, knitr  
* R build toolchain: Rtools(windows) or XCode (mac) or `r-base-dev`
See Packages in a nutshell and Setting up your system...  

---
### Package documentation

types of documentation: about the package metadata
DESCRIPTION file
dependencies
licenses
version
object documentation roxygen
workflow

#### Learning Objectives
At the end of this module the successful learner will be able to:  
*   
*   
*   
*   

#### Prerequisites

---

### five

Outline

#### Learning Objectives
At the end of this module the successful learner will be able to:  
*   
*   
*   
*   

#### Prerequisites

---

### six

Outline

#### Learning Objectives
At the end of this module the successful learner will be able to:  
*   
*   
*   
*   

#### Prerequisites



 