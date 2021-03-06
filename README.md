# ![nf-core/featurecounts](docs/images/featurecounts_logo.png)

[![Build Status](https://travis-ci.com/nf-core/featurecounts.svg?branch=master)](https://travis-ci.com/nf-core/featurecounts)
[![Nextflow](https://img.shields.io/badge/nextflow-%E2%89%A50.30.2-brightgreen.svg)](https://www.nextflow.io/)
[![install with bioconda](https://img.shields.io/badge/install%20with-bioconda-brightgreen.svg)](http://bioconda.github.io/)
[![Docker Automated build](https://img.shields.io/docker/automated/nfcore/featurecounts.svg)](https://hub.docker.com/r/qbicsoftware/icgc-featurecounts)
[![https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg](https://www.singularity-hub.org/static/img/hosted-singularity--hub-%23e32929.svg)](https://singularity-hub.org/collections/1315)
[![DOI](https://zenodo.org/badge/142166753.svg)](https://zenodo.org/badge/latestdoi/142166753)


This pipeline uses featureCounts on cancer datasets from ICGC and generates count matrices, similar to what [nf-core/RNAseq](https://github.com/nf-core/RNAseq) does. Users can specify a ICGC Manifest file with object ids, which will then be converted to encrypted S3 URLs. The pipeline then uses the provided GTF file to generate count matrices for all files in the manifest.

### Introduction

The pipeline is built using [Nextflow](https://www.nextflow.io), a workflow tool to run tasks across multiple compute infrastructures in a very portable manner. It comes with docker / singularity containers making installation trivial and results highly reproducible.


### Documentation
The ICGC-FeatureCounts pipeline comes with documentation about the pipeline, found in the `docs/` directory:

1. [Installation](docs/installation.md)
2. Pipeline configuration
    * [Local installation](docs/configuration/local.md)
    * [Adding your own system](docs/configuration/adding_your_own.md)
3. [Running the pipeline](docs/usage.md)
4. [Output and how to interpret the results](docs/output.md)
5. [Troubleshooting](docs/troubleshooting.md)

### Credits
This pipeline was written by Alexander Peltzer ([apeltzer](https://github.com/apeltzer)) at [QBiC](apeltzer.github.io) with some help from Paolo DiTommaso ([pditommaso](https://github.com/pditommaso)) and the Nextflow community.
