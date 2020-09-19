# AM_AMP

## Using this repository

This repository contains scripts and code to create a phylogenetic tree for a family of AMP's discovered in Acropora millepora.  It was published as Figure 3 in;

> AmAMP1 from Acropora millepora and damicornin define a family of coral-specific antimicrobial peptides related to the Shk toxins of sea anemones

> https://doi.org/10.1016/j.dci.2020.103866



To obtain raw data required to run these scripts you should do the following;

1. Checkout this repository 
```bash
git clone https://github.com/iracooke/amamp_pub.git
```
2. Download the raw data and unpack it from within the project repository.
```bash
cd amamp_pub
wget 'https://cloudstor.aarnet.edu.au/plus/s/zjlFSUchshirLUt/download' -O data.tgz
tar -zxvf data.tgz
```

### Data Processing

- [Initial Transcriptome Assembly](hpc/Assembly)
- [Symbiont Transcript Removal](hpc/psytrans)
- [Clustering transcripts and counting assigned reads](hpc/corset)
- [Functional Annotation with Trinotate](hpc/trinotate)

### Statistical Analysis and Visualisation

- [Gene Annotation](01_annotate.md)
- [Differential Expression Analysis](02_deseq.md)
- [Analysis of Polyp Activity Observations](03_polyp_activity.md)

