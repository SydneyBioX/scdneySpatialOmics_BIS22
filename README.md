# scdneySpatialOmics_BIS22
Materials for 'Unlocking single cell spatial omics analyses with scdney' workshop presented at BioInfoSummer 2022

## Requirements

Before coming to the workshop, you must have a functioning R installation, paired with your favourite IDE and git.

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
