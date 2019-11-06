# PharmRF
PharmRF is a new scoring function to choose the best crystal structure for pharmacophore-based virtual screening. 

About PharmRFscoring function

PharmRF is a pharmacophore-based scoring function for selecting the best crystal structure with high possibilities of ensuring high enrichment rates in pharmacophore-based virtual screening. PharmRF trained on PDBbind v2018 protein-ligand complex dataset, employs random forest (machine learning) approach to correlate protein pocket descriptors (physicochemical properties of ligand binding sites in the protein) and pharmacophore features involved in protein-ligand interactions (physicochemical properties of ligand) to correlate binding affinity. Protein-ligand complexes which secured top  2 orders of PharmRF score has achieved 87.5 % success rate compared to its coupling to resolution and affinity factors, in eight datasets. PharmRF is very robust and fast to identify the best protein-ligand complex templates by thorough pruning of all the PDB entries available for a particular protein of interest. 

Publication:

Manuscript submitted.

Prerequisites for running pharmrf.sh (shell file):

1. fpocket program: please follow the instructions to install Fpocket locally in your computer. 

Manual: http://fpocket.sourceforge.net/manual_fpocket2.pdf
Download: https://sourceforge.net/projects/fpocket/files/fpocket-1.0/fpocket-src-1.0/

2. PLIP (Protein Ligand Interaction Profiler): please follow the instructions to install PLIP locally in your computer. 

Download and Instructions: https://github.com/ssalentin/plip

Prerequisite for running WEKA Pharmrf.model (model file):

3. WEKA: Download and install Weka v3.8 (stable version) according to your OS and system architecture.
https://www.cs.waikato.ac.nz/ml/weka/downloading.html

Compilations:

Linux and Ubuntu - fpocket v1.0 and PLIP v1.0

Any OS - Weka v3.8 (stable version)

Manual and example sets:

Please follow the manual and execute on example sets.

Authors:

Sivakumar Prasanth Kumar, Chirag Patel, Rakesh Rawal and Himanshu Pandya
