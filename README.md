# PhloMICOM
PhyloMICOM is an extension of the MICOM package, designed to improve the accuracy and efficiency of microbial community simulations by incorporating phylogenetic relationships. This project introduces a modified version of the community.py file from the MICOM package, along with additional scripts and data for analysis.

micom Folder:
This folder contains the original MICOM package, with a key modification to the community.py file. The modification, known as PhyloMICOM, pools the metabolic models of phylogenetically related organisms at the order level. This allows for more accurate and phylogenetically-informed simulations of microbial communities.

Building community models:
##
<tab><tab>
from micom.data import test_db

from micom.workflows import build

manifest = build(data, out_folder="models", model_db=test_db, cutoff=0.0001, threads=2)
##


analysis Folder:
This folder includes a collection of Python scripts used to analyze microbial communities. These scripts are tailored to work with the PhyloMICOM framework and provide tools for various types of analyses, such as sensitivity testing, growth rate prediction, and statistical evaluations.

data Folder:
The data folder contains all the input datasets used for running simulations and the corresponding output data generated by PhyloMICOM. This includes metagenomic data, configuration files, and simulation results. The input data is structured to be easily accessible for rerunning or extending the analyses performed in this project.
