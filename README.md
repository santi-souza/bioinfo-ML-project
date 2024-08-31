# Bioactivity Prediction Project

This repository contains a bioinformatics project focused on predicting the biological activity of compounds against the target protein Acetylcholinesterase. 
The project follows the tutorial series by Data Professor (https://github.com/dataprofessor), which guides through the process of data collection, exploratory data analysis, molecular descriptor calculation, and regression model building.

## Project Highlights

- **Data Collection:** Downloaded and pre-processed bioactivity data from the ChEMBL database.
- **Exploratory Data Analysis (EDA):** Performed EDA on Lipinski molecular descriptors.
- **Model Building:** Built and evaluated regression models to predict pIC50 values using molecular descriptors.

This project is divided into multiple parts, each addressing a different stage of the bioinformatics pipeline:
1. **Data Collection:** Downloaded and pre-processed biological activity data from the ChEMBL database.
2. **Lipinski Descriptors & EDA:** Calculated molecular descriptors and performed exploratory data analysis (EDA).
3. **Target Protein Selection & Dataset Preparation:** Focused on Acetylcholinesterase due to its larger dataset and prepared data for modeling.
4. **Regression Model Building:** Built a regression model to predict pIC50 values.
5. **Model Comparison:** Used the LazyPredict library to compare various regression models.

## PaDEL Descriptor

The molecular descriptors used in this project were calculated using the PaDEL-Descriptor software. 
PaDEL-Descriptor is a powerful tool that calculates 1875 molecular descriptors and 12 types of fingerprints, totaling 16092 bits. These descriptors are essential for understanding the properties of molecules and include:

- **1D, 2D Descriptors:** 1444 descriptors capturing structural and compositional information.
- **3D Descriptors:** 431 descriptors capturing spatial and geometric information.
- **Fingerprints:** 12 types of fingerprints, which are binary representations of molecular substructures.
  
The descriptors and fingerprints are calculated using The Chemistry Development Kit (CDK) along with additional specialized descriptors such as:

- Atom type electrotopological state descriptors
- Crippen's logP and MR
- Extended topochemical atom (ETA) descriptors
- McGowan volume
- Molecular linear free energy relation descriptors
- Ring counts
- Chemical substructures identified by Laggner
- Fingerprints identified by Klekota and Roth

These molecular descriptors are key to building the predictive models used in this project.

## Acknowledgments

This project was guided by the tutorial series from the Data Professor. The videos provide a step-by-step approach to building a bioinformatics project from scratch.

- **YouTube Series:** [Data Professor Bioinformatics Project](https://www.youtube.com/watch?v=plVLRashaA8&list=PLtqF5YXg7GLlQJUv9XJ3RWdd5VYGwBHrP&index=1)
- **GitHub Repository:** https://github.com/dataprofessor
- **PaDEL descriptor**: http://www.yapcwsoft.com/dd/padeldescriptor/
- **PaDEL paper**: https://onlinelibrary.wiley.com/doi/full/10.1002/jcc.21707
