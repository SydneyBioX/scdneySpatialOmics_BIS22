# Unlocking single cell spatial omics analyses with `scdney`
Materials for 'Unlocking single cell spatial omics analyses with `scdney`' workshop presented at [BioInfoSummer 2022](https://bis.amsi.org.au/program/).

## Prerequisites

Before coming to the workshop, you must have the latest version of R installed 
(or at least version 4.2), paired with your favourite IDE (e.g. 
[RStudio](https://posit.co/download/rstudio-desktop/)) and/or git for 
downloading the workshop materials.

### Installing `scdney`

`scdney` is a collection of packages developed by researchers at the Sydney 
Precision Data Science Centre. As a result of the many packages contained in 
this collection, `scdney` contains several dependencies and can take a while to 
install, attendees should have installed it prior to the beginning of the 
workshop.

`scdney` can be installed as follows.

```r
# if BiocManager or remotes packages are not installed
install.packages(c("BiocManager","remotes"))

# install scdney
BiocManager::install("SydneyBioX/scdney")
# test the installation by loading scdney
library(scdney)
```

### Workshop structure

First, download the files in this Github repository by either cloning the 
repository or by downloading the files directly into a directory on your
computer.

Next, we will worth through two key examples with datasets.

### Dev container option

If you were unable to install any packages before the workshop but happen to 
have Docker installed, it may be quicker to use a VS Code dev container to get
started.

1. Clone the repo and run the following.
    ```bash
    docker build -t scdney_image .
    ```
    While this is running (should take >10 mins), install VS Code, and its R 
    and dev container extension.

2. Run and start the image that docker has built.

    ```bash
    docker run -d --name scdney_container scdney_image
    docker start scdney_container
    ```

    Now you should have a container with the `scdney` environment installed.  
3. Open VS Code and open a folder inside the container.

You are now ready to start running the workshop!

### Contact

Shila Ghazanfar shila.ghazanfar@sydney.edu.au

Nicholas Robertson nicholas.robertson@sydney.edu.au

Ellis Patrick ellis.patrick@sydney.edu.au
