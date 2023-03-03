# Installation of R and R-Studio


![](https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/R_logo.svg/200px-R_logo.svg.png)



## Installing R

The first step is to install R. You can download and install R from
the [Comprehensive R Archive Network](https://cran.r-project.org/)
(CRAN). 

Windows:
Open the [Comprehensive R Archive Network](https://cran.r-project.org/). 
Click on “CRAN”. You’ll see a list of mirror sites, organized by country. 
Select a site near you. 
Click on “Windows” under “Download and Install R”. 
Click on “base”. 
Click on the link for downloading the latest version of R (an .exe file). 
When the download completes, double-click on the .exe file and answer the usual questions. 

Mac:
Open the [Comprehensive R Archive Network](https://cran.r-project.org/). 
Click on “CRAN”. 
You’ll see a list of mirror sites, organized by country. 
Select a site near you. 
Click on “MacOS X”. 
Click on the .pkg file for the latest version of R, under “Files:”, to download it. 
When the download completes, double-click on the .pkg file and answer the usual questions. 


## Installing RStudio

The next step is to install **RStudio**, a free and open-source integrated development environment (IDE) for R. You can use it for viewing and running R scripts. We install the latest preview version of the software:

Go to [RStudio Download](https://rstudio.com/products/rstudio/download/preview/)
Click the Download RStudio Desktop button.
Select the installation file for your system.
Run the installation file.


## R Basics


Two key things you need to know about R is that you can get help for a function using `help` or `?`, like this:

```{r,eval=FALSE}
?install.packages
help("install.packages")
```

and the hash character represents comments, so text following these
characters is not interpreted:

```{r}
##This is just a comment
```

## Installing R Packages

The first R command we will run is `install.packages`. 

An R package is a collection of functions, data, and documentation that extends the capabilities of base R. 
Many of these functions are stored in CRAN. You can easily install packages from within RStudio if you know
the name of the packages. 

As an example, we are going to install the
package `dplyr` which we use in our first data
analysis examples: 

```{r,eval=FALSE}
install.packages("dplyr")
```

We can then load the package into our R sessions using the `library` function:

```{r}
library(dplyr)
```

From now on you will see that we sometimes load packages without
installing them. This is because you only need to install a package once, 
but you need to reload it with the command `library` every time you start 
a new R session.

If you try to load a package and get an error, it probably means you need to
install it first.

Review the [dplyr-documentation](https://cran.r-project.org/web/packages/dplyr/vignettes/dplyr.html) to get an overview about the different functionalities of this package.
