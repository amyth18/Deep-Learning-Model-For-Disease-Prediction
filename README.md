# Overview
As part of our final project coursework for CS598 Deep Learning for Healthcare, Spring 2022, we have implemented and evaluated a deep learning model from scratch as proposed in the paper titled [A disease inference method based on symptom extraction and bidirectional Long Short Term Memory networks](https://pubmed.ncbi.nlm.nih.gov/31301375/) by Donglin Guo et al. The main idea of the paper is to predict on-set of diseases by extracting symptoms from the clinical text history of patients using Bi-LSTM networks. The following diagram captures the high level architecture of the proposed model.

<p align="center">
  <img src="https://user-images.githubusercontent.com/8692284/166911831-85412059-07db-48b5-ab20-f43217234930.png">
</p>

# Pre-Requesites
## Data
1. To train and evaluate the models you will need access to the MIMIC III dataset version 1.4. The dataset can be obtained from the [physionet.org](https://physionet.org/content/mimiciii/1.4/). You will need to first register on the website (if you don't already have an account) and complete the CITI training before you can request for access.
2. The code requires the dataset to be stored on Google drive. Please refer to the pre-requisite sections of individual notebooks for specific instructions on setting up folder paths. If you choose to use a different storage service then you will have to make necessary changes to load data sections in the notebooks, every thing else should remain same after that.
## Compute
1. We have used the Google's colab environment to train and evaluate all our models. You can can launch the notebooks in colab environment by simply clicking on the "colab" button on each notebook.
2. You will need GPU support for all running all notebooks. We have tested these notebooks using colab pro+ acccount as the compute and memory requrements are quite intensive for training these models.
3. We belive the code should run on any jupyter notebook environments, but we have not done any testing from our side.

# Code Organization
The following table provides the top level navigation map for this repository, please refer to the individual notebooks for more detailed documentation on the model architecture, data processing, training and evaluation. Each notebook is self-contained and can be run from start to end to reproduce the results.

| File | Description |
| --- | --- |
|[Main_Prediction_Model_Final_Submission.ipynb](https://github.com/amyth18/CS598-Deep-Learning-Final-Project/blob/main/Main_Prediction_Model_Final_Submission.ipynb) | <ul><li>This is the <b>main file</b>, it contain end-to-end implementation of the proposed model and methods. <li> Also contains implementation for 2 out of the 3 baseline models we evaluate in this study as they share data processing steps.</ul> |
| [Other_Baseline_Models.ipynb](https://github.com/amyth18/CS598-Deep-Learning-Final-Project/blob/main/Other_Baseline_Models.ipynb) | <ul><li>Contains implementaion for DeepLabeler, the 3rd baseline model we use in our evaluation study.
| [Data_Cleaning.ipynb](https://github.com/amyth18/CS598-Deep-Learning-Final-Project/blob/main/Data_Cleaning.ipynb) | <ul><li>Utility code for data cleaning, exploration etc.</ul>
