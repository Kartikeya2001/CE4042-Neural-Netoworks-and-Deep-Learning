# CE-CZ4042-Neural-Networks-and-Deep-Learning

# Group Project
> In recent times, social networking has become a huge part of our day-to-day activities. From WhatsApp to Instagram, we always stay connected and updated about the people whom we care about. One such social networking service is Twitter that has connected people from different parts of the world and supported numerous businesses. On this platform, users post and interact with messages known as “tweets”. Users are exposed to tweets that are of various categories such as excited, angry, sad, happy, etc. Thus, our team felt the need to identify the sentiment of a given tweet to help the user identify the type of content they are being exposed to on a daily basis. Hence, we decided to use the Long Short Term Memory networks to fulfill our mission. 

The original data can be found in `/data/Original Data`. To follow along in the training process, please follow the following order:
- `/scripts/Data-Cleaning.ipynb`
- `/scripts/Exploratory-Data-Analysis.ipynb`
- `/scripts/Feature-Engineering.ipynb`
- `/scripts/LSTM-Vanilla-First-Trial.ipynb`
- Following the above Jupyter Notebook, please execute the following files for model construction, training and tuning.
```bash 
python LSTM-Trial-Architectures.py       # Train different model architectures to see model progression
python LSTM-Final.py                     # Train the final model architectures ( with 9 and 3 labels )
python Hyperparameter-Tuning.py          # Identify the best Hyperparameters for the final model
```
- For post - processing, execute `/scripts/Postprocessing.ipynb`


# Programming Assignment
## Part A: Classification Problem

• DNN to classify the GTZAN dataset: http://marsyas.info/downloads/datasets.html which includes 1000 audio tracks, spanning 30 seconds each

• The dataset has been pre-processed and 57 features has been extracted into the features_30_sec.csv

• There are 10 different genres to classify: blues, classical, country, disco, hip-hop, jazz, metal, pop, reggae and rock


## Part B: Regression Problem

• The aim is to predict housing prices in Singapore from related features (#9)

• Numeric features: dist_to_nearest_stn, dist_to_dhoby, degree_centrality, eigenvector_centrality, remaining_lease_years, floor_area_sqm

• Categorical features: month, flat_model_type, storey_range

• Divided the dataset into Train data: up to year 2020; Test data: for year 2021; One-hot encoding for categorical variables

• Used an embedding layer after the one-hot embeddings for categorical variables inorder to improve prediction

• Implemented Recursive Feature Extraction (RFE) from sratch to remove irrelevant features one-by-one

