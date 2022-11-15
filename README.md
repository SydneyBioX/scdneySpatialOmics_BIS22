# scdneySpatialOmics_BIS22
Materials for 'Unlocking single cell spatial omics analyses with scdney' workshop presented at BioInfoSummer 2022

## Prerequisites

Before coming to the workshop, you must have a functioning R installation, paired with your favourite IDE and git.

### `scdney` installation

Additionally, since `scdney` contains many dependencies and can take a while to install, atendees should have installed it prior to the beggining of the workshop.

It can be installed as follows.

```r
# if BiocManager or remotes packages are not installed
install.packages(c("BiocManager","remotes"))

# install scdney
BiocManager::install("SydneyBioX/scdney")
# test the installation by loading scdney
library(scdney)
```

### Dev Container

If you were unable to install any packages before the workshop but happen to have docker installed, it may be quicker to use a vscode dev container to get started.

1. Clone the repo and run the following.
  ```sh
  docker build -t scdney_image .
  ```
  While this is running (should take >10 mins), install vscode and it's R and dev container extension.

2. Run and start the image that docker has built.

  ```r
  docker run -d --name scdney_container scdney_image
  docker start scdney_container
  ```

Now you should have a conatiner with the `scdney` environment installed.  
