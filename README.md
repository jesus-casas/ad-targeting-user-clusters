# AD Targeting Users For Sponsor

## Project Summary
This project focuses on optimizing ad targeting strategies by identifying distinct user segments within a social media audience. By analyzing behavioral data and posted content from 1,000 synthetic users, I applied unsupervised machine learning techniques to group users into four meaningful clusters. These clusters reveal unique preferences and engagement patterns, enabling sponsors to tailor their advertising campaigns for maximum effectiveness.

## Skills and Technologies
This project demonstrates proficiency in the following areas:

*   **Programming Language**: R
*   **Data Analysis & Manipulation**: `dplyr`, `readr`, `gtools`
*   **Machine Learning**: K-Means Clustering (`cluster`), Principal Component Analysis (PCA)
*   **Data Visualization**: `ggplot2`, `factoextra`, `gridExtra`, `patchwork`
*   **Key Skills**: 
    *   Data Preprocessing & Cleaning
    *   Feature Engineering (One-hot encoding, Scaling)
    *   Unsupervised Learning
    *   Statistical Analysis & Visualization

## Dataset Characteristics
The dataset consists of 1,000 entries in `synthetic social media users.csv`. Each row represents a unique user, including demographic and behavioral data. Additionally, the last image posted by each user is available in the "posted images" folder, named "imageX.jpg" (where X corresponds to the user ID).

## Steps Taken
### Step 1: Exploring the Dataset
Analyzed the dataset structure, checked for missing values, and identified numerical vs. categorical features.

### Step 2: Data Preprocessing
Cleaned the data and applied one-hot encoding to convert categorical variables into a format suitable for analysis.

### Step 3: Standardization
Scaled the dataset to ensure that all features contribute equally to the distance calculations used in clustering.

### Step 4: K-Means Clustering
Implemented the K-Means algorithm to partition users into 4 distinct clusters based on their shared characteristics.

### Step 5: Evaluation and Visualization
Visualized the clusters using PCA (Principal Component Analysis) to interpret the results and understand the distinct traits of each user group.
