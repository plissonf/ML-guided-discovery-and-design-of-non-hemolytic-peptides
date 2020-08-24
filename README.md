# ML-guided-discovery-and-design-of-non-hemolytic-peptides

This repository accounts for the development of binary classification models to predict haemolytic nature (HemoPI-1) and haemolytic activity (HemoPI-2, HemoPI-3) of peptide sequences from their physicochemical properties. It is divided into 5 folders (DATA, DESCRIPTORS, MODELS, RESULTS, SCRIPTS).

DATA includes all peptide sequences (HemoPI-1, HemoPI-2, HemoPI-3, total APD, HAMP, RPS) in fasta files as well as some information related to webscraping the Antimicrobial Peptide Database (November 2019)

DESCRIPTORS has the raw, cleaned and normalised datasets (.csv) with physicochemical properties derived from peptide sequences.

MODELS provides all 9 top models (3 per HemoPI dataset), available in pickled (.pkl) formats

RESULTS gathers the predictions from all 9 models applied to HemoPI model datasets, HemoPI validation datasets, APD dataset, HAMP dataset and the dataset of generated inliers (RPS) as well as the results from univariate/multivariate outlier detection methods.

SCRIPTS contains 6 Jupyter notebooks scripts written in Python 3.6+ ordered in the development of the research project;
- 1-Antimicrobial Peptide Database APD3 Webscraper & Cleanser.ipynb
- 2-Calculator of Descriptors (modlamp) from peptide primary sequences.ipynb
- 3-Classification models on Hemolytik datasets with 56 modlamp descriptors.ipynb
- 4-Multivariate Outlier Detection algorithms applied to HemoPI, APD, HAMP datasets.ipynb
- 5-Predicting hemolytic activity and outliers in testing and de novo datasets.ipynb.ipynb
- 6-Generating random peptide sequences (RPS) with APD inliers amino acid composition.ipynb
