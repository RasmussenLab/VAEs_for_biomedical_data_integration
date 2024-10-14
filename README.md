# VAEs for biomedical data integration

## Summary: 
This is the repository for the paper "On the use of VAEs for biomedical data integration". This is mostly intended to be a data repository, and it also contains a short tutorial on how to reproduce the main findings of the paper. For a detailed explanation of the Multiomics Variational Autoencoder (MOVE) we refer the reader to the MOVE repository (https://github.com/RasmussenLab/MOVE).

![Main image](https://raw.githubusercontent.com/RasmussenLab/VAEs_for_biomedical_data_integration/master/images/Image_main.png)

## Folder structure: 
- **configs:** Configuration files used to build the models using MOVE.
- **images:** Images for the repository.
- **models:** Final trained MOVE model weights used for the paper.
- **scripts:** Folder containing:
  - **MOVE**. Exact folder structure and files used when running the analysis.
  - *AMSC_MOVE.ipynb*: Main notebook of the project. Contains the data preprocessing steps and data analysis on both synthetic data and AMSC data.
  - *Tutorial_AMSC_MOVE.ipynb*: Tutorial notebook on how to install MOVE, create a synthetic dataset, analyze the latent space and identify associations.




