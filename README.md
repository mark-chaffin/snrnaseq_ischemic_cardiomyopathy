# Single Nucleus RNA sequencing in Ischemic Cardiomyopathy Reveals Common Transcriptional Profile Underlying End-Stage Heart Failure

This repository contains main analysis code used in the project "Single Nucleus RNA sequencing in Ischemic Cardiomyopathy Reveals Common Transcriptional Profile Underlying End-Stage Heart Failure". The project consists of snRNA-seq of 99,684 nuclei from the left ventricle of 15 patients (7 ischemic cardiomyopathy and 8 non-failing). Processed single-nuclei RNA-seq data can be found at https://singlecell.broadinstitute.org/single_cell/study/SCP1849/ and raw sequencing data is available to authorized users via dbGaP under accession phs001539.v4.p1.

Code is separated into 3 folders:
1. Map construction -- code to take the raw CellRanger and CellBender output, perform nuclei QC, and construct a global map.
2. Differential expression testing -- code to test for Marker Genes (differentially expressed between clusters) and Disease Genes (differentially expressed between ischemic cardiomyopathy and non-failing, by cell type).
3. Sub-clustering endothelial cells -- code to perform the sub-clustering analysis of endothelial cells.

Within each folder, code is stored as sequential jupyter notebooks for main analyses.

Additional analyses reported in the manuscript (e.g., compositional testing, pathway enrichment, cell-cell communication) were performed using default code from the specific tools reported in the methods. No additional custom code was written for these analyses beyond basic data manipulation to format the data for input into these well documented tools. The combined analysis of DCM, HCM, ICM, and NF samples
