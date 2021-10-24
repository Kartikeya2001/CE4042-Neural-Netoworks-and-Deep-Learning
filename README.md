# Programmimg Assignment

## Part A: Classification Problem

• DNN to classify the GTZAN dataset: http://marsyas.info/downloads/datasets.html which includes 1000 audio tracks, spanning 30 seconds each
• The dataset has been pre-processed and 57 features has been extracted into the features_30_sec.csv
• There are 10 different genres to classify: blues, classical, country, disco, hip-hop, jazz, metal, pop, reggae and rock

## Part B: Regression Problem

• The aim is to predicting housing prices in Singapore from related features (#9)
• Numeric features: dist_to_nearest_stn, dist_to_dhoby, degree_centrality, eigenvector_centrality, remaining_lease_years, floor_area_sqm
• Categorical features: month, flat_model_type, storey_range
• Divided the dataset into Train data: up to year 2020; Test data: for year 2021; One-hot encoding for categorical variables
• Used an embedding layer after the one-hot embeddings for categorical variables inorder to improve prediction
• Implemented Recursive Feature Elimination (RFE) from sratch to remove irrelevant features one-by-one

