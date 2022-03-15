# PharmRF
PharmRF is a new scoring function to choose the best crystal structures for pharmacophore-based virtual screening. 

**PharmRF scoring function**

Structure-based pharmacophore models are often developed by selecting a single protein-ligand complex with good resolution and better binding affinity data which prevents the analysis of other structures having a similar potential to act as better templates. PharmRF is a pharmacophore-based scoring function for selecting the best crystal structures with the potential to attain high enrichment rates in pharmacophore-based virtual screening prospectively. The PharmRF scoring function is trained and tested on the PDBbind v2018 protein-ligand complex dataset and employs a random forest regressor to correlate protein pocket descriptors and ligand pharmacophoric elements with binding affinity. PharmRF score represents the calculated binding affinity which identifies high-affinity ligands by thorough pruning of all the PDB entries available for a particular protein of interest with a high PharmRF score. Ligands with high PharmRF scores can provide a better basis for structure-based pharmacophore enumerations with a better enrichment rate. Evaluated on 10 protein-ligand systems of the DUD-E dataset, PharmRF achieved superior performance (average success rate: 77.61 %, median success rate: 87.16 %) than Vina docking score (75.47 %, 79.39 %). PharmRF coupling to protein-ligand complex sets with experimental binding affinity showed somewhat better performance (average success rate: 51.94 %, median success rate: 51.51 %) than actual experimental affinity (34.43 %, 29.16 %) demonstrating that PharmRF calculations on the complete set of available complexes 
will gauge complexes with high enrichments comparatively. The PharmRF scoring function was further evaluated using the CASF-2016 benchmark set yielding a moderate correlation of 0.591 with experimental binding affinity, similar in performance to 25 scoring functions tested on this dataset, necessitating further improvements in the scoring ability. Independent assessment of PharmRF on 8 protein-ligand systems of LIT-PCBA dataset exhibited average and median success rates of 57.55 % and 74.72 %, respectively with 4 targets attaining success rate more than 90 %. The PharmRF scoring model, scripts, and related resources can be accessed here.


**Publication:**

Kumar SP et al. (2020). PharmRF machine-learning scoring function to identify the best protein-ligand complexes for structure-based pharmacophore screening with high enrichments. Journal of Computational Chemistry, 10.1002/jcc.26840

**Prerequisites for running pharmrf.sh (shell file):**

1. fpocket program: please follow the instructions to install Fpocket locally in your computer. 

      Manual: http://fpocket.sourceforge.net/manual_fpocket2.pdf

      Download: https://sourceforge.net/projects/fpocket/files/fpocket-1.0/fpocket-src-1.0/

2. PLIP (Protein Ligand Interaction Profiler): please follow the instructions to install PLIP locally in your computer. 

      Download and Instructions: https://github.com/ssalentin/plip

**Prerequisite for running WEKA Pharmrf.model (model file):**

3. WEKA: Download and install Weka v3.8 (stable version) according to your OS and system architecture.
https://www.cs.waikato.ac.nz/ml/weka/downloading.html

**Compilations:**

Linux and Ubuntu - fpocket v3.0 and PLIP v1.4.4

Any OS - Weka v3.8 (stable version)

**Manual and example sets:**

Please follow the manual and execute on example sets.

**Video Demonstration:**

https://www.youtube.com/watch?v=oPy5NlDtP9g

**Developer and Primary contact:**

Prasanth Kumar (prasanthbioinformatics[at]gmail.com). 
