
# Scripts
## Jupyter notebooks:
The code is organized in the following ipython jupyter notebooks:
- *On_the_use_of_VAEs_for_biomedical_data_integration.ipynb*: Main notebook of the project.
- *MOVE_edits.ipynb*: We added small edits to MOVE's code for this particular project. This notebook keeps track of them.
- *Tutorial_VAEs_for_biomedical_data_integration.ipynb*: Notebook guiding the reader through the main findings of the project. This is done by creating a synthetic dataset and performing the analyses as done in the paper.
- *Toy_models_Elhage_et_al.ipynb*: Adaptation of the code in the colab notebook from Anthropic's paper by Elhage et al. Toy models of superposition. The notebook shows the behaviour of a simple autoencoder when compressing inputs under different correlation regimes.

For specific details regarding MOVE we refer the user to the [MOVE repository](https://github.com/RasmussenLab/MOVE).

## config

Config files to create, train and evaluate the MOVE models used in this project are provided. Please note that the config file system used in MOVE is based on [hydra](https://hydra.cc/docs/intro/). In some cases the default hyperparameters were overridden dynamically, providing them when calling specific move-dl functions in command-line style. For more information please follow the notebooks. 


