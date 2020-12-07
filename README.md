# PharmRF
PharmRF is a new scoring function to choose the best crystal structures for pharmacophore-based virtual screening. 

PharmRFscoring function

Structure-based pharmacophore models are often developed by selecting a single protein-ligand complex with good resolution and better binding affinity data which prevents the analysis of other structures having a similar potential to act as better templates. PharmRF is a pharmacophore-based scoring function for selecting the best crystal structures with the potential to attain high enrichment rates in pharmacophore-based virtual screening prospectively. The PharmRF scoring function is trained and tested on the PDBbind v2018 protein-ligand complex dataset and employs a random forest regressor to correlate protein pocket descriptors and ligand pharmacophoric elements with binding affinity. PharmRF score represents the calculated binding affinity which identifies high-affinity ligands by thorough pruning of all the PDB entries available for a particular protein of interest with a high PharmRF score. Ligands with high PharmRF scores can provide a better basis for structure-based pharmacophore enumerations with a better enrichment rate. Evaluated on 10 protein-ligand systems, PharmRF achieved superior performance (average success rate: 77.61 %, median success rate: 87.16 %) than experimental binding affinity (34.43 %, 29.16 %), and Vina docking score (75.47 %, 79.39 %). The PharmRF scoring model, scripts, and related resources can be accessed here.

Publication:

Kumar SP et al. (2020). PharmRF machine-learning scoring function to identify the best protein-ligand complexes for structure-based pharmacophore screening with high enrichments. Submitted.

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

Video Demonstration:

Click on this image for PharmRF demonstration (directs to YouTube)

[![IMAGE ALT TEXT](https://i.ibb.co/Vmngg6Y/PharmRF.jpg)](https://youtu.be/oPy5NlDtP9g "PharmRF Demonstration")

Authors:

Sivakumar Prasanth Kumar, Chirag Patel, Rakesh Rawal and Himanshu Pandya
