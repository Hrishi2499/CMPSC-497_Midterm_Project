# CMPSC-497_Midterm_Project

There are two python notebooks Emotion_Detection_(Data_Collection).ipynb and Emotion_Detection_Model_Training.ipynb.

# Data Collection:
This notebook reads the combined_emotions and the train, test and val txt files. It has some visualizations, used for EDA.

It outputs the emotion_data_alt.csv dataset for model training.

# Model training
This notebook reads the dataset emotion_data_alt.csv as a Pandas Dataframe and performs pre-processing on it, to get tokenized and padded sequences and LabelEncoded targets.

The GloVe embeddings are loaded from the embedding file, I have added code to download and unzip the embeddings. The file path must be specified accordingly to load the embeddings.

Each of the four models decribed in the report are defined and compiled and can be trained. I have trained them on the Google Colabs python environment with T4 GPU.
Post training and evaluation, the model can be saved.

Towards the end, hyper-parameter tuning code is provided, which was used to optimize some of the hyperparameters.
