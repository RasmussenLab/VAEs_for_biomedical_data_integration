# VAEs for biomedical data integration

## Summary: 
This is the repository for the paper _On the use of VAEs for biomedical data integration_. It contains the code and configs used in the paper, but also includes a short tutorial on how to reproduce our main findings. For a detailed explanation of the Multiomics Variational Autoencoder (MOVE) we refer the reader to the [MOVE repository](https://github.com/RasmussenLab/MOVE). Small code edits were added for this project, which are described in a separate notebook.

![Main image](images/Image_main.png)

**Figure 1. Latent space visualization**. *a) Latent space representation of all samples color coded by their normalized value of the feature Continuous_B1. b) Idem for Continuous_B_2. c) Movement of all samples after perturbing positively the feature Continuous_B1. Note that, since both features are positively correlated, the perturbation brings samples towards a region where feature values for both variables are higher.*

## Repository structure: 
- **configs:** The MOVE framework uses [hydra](https://hydra.cc/docs/intro/) to manage and define most hyperparameters related to model architecture and training. These hyperparameters are specified in a number of configuration files. This folder contains the baseline configuration files we used to build the models.
- **images:** Images for the repository.
- **scripts:** Folder containing:
  - *MOVE_edits.ipynb*. Notebook explaining what files in the MOVE source code were modified for this project and how.
  - *AMSC_MOVE.ipynb*: Main notebook of the project. Contains the data preprocessing steps and data analysis on both synthetic data and AMSC data.
  - *Tutorial_VAEs_for_biomedical_data_integration.ipynb*: notebook on how to install MOVE, create a synthetic dataset, analyze the latent space, identify associations and visualize the perturbation effects on sample embeddings. The following hyperlink opens it as a Google Colab notebook:

      [![open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/RasmussenLab/VAEs_for_biomedical_data_integration/blob/main/scripts/Tutorial_VAEs_for_biomedical_data_integration.ipynb)  
  - *Toy_models_Elhage_et_al.ipynb*: Adaptation of the code in [the colab notebook](https://colab.research.google.com/github/anthropics/toy-models-of-superposition/blob/main/toy_models.ipynb) from Anthropic's paper by Elhage et al. [Toy models of superposition](https://transformer-circuits.pub/2022/toy_model/index.html). The notebook shows the behaviour of a simple autoencoder when compressing inputs under different correlation regimes.
    
## Other files:
Heavier files (e.g. model weights for the 24 refits of the model architecture used to identify associations) were not uploaded here due to their size. Note that different runs will yield different sets of weights, and hence different looking latent spaces. The paper was written so that the underlying principles presented are reproducible regardless of the dataset or machine used.


