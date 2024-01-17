# nf-core_training
Training material for nf-core workflows in metagenomics

## Workflows for metagenomics
- nf-core/mag
- nf-core/taxprofiler

## Pre-requirement
### Install software and packages 
Via conda with the `environment.yml` file

### Install and test workflows
```
nextflow run nf-core/mag -profile test,YOURPROFILE --outdir <OUTDIR>
```

## Download databases
- mOTUs
- metaPhlAn
- Kraken/Bracken
- Centrifuge

## How to run
### mag
```
nextflow run nf-core/mag -profile <docker/singularity/podman/shifter/charliecloud/conda/institute> --input '*_R{1,2}.fastq.gz' --outdir <OUTDIR>
```

### taxprofiler
```
nextflow run nf-core/taxprofiler --input samplesheet.csv --databases databases.csv --outdir <OUTDIR> -profile docker --run_<TOOL1> --run_<TOOL2>
```
