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

![Cluster Analysis](./images/cluster_analysis.png)

### Characteristics of Each Cluster

Based on the analysis of 1,000 synthetic users four distinct segments were identified:

**Cluster 1: "The Power Users" (Young & Highly Active)**

-   **Demographics:** Youngest group (Avg Age: ~25).
-   **Behavior:** Extremely high engagement with ~60 hours/month active, ~30 posts, and ~1198 likes.
-   **Tech:** Predominantly Mobile (iOS) users.
-   **Social:** Highest social connectivity with ~447 friends.

**Cluster 2: "The Casual Observers" (Older & Less Active)**

-   **Demographics:** Oldest group (Avg Age: ~60).
-   **Behavior:** Lowest engagement with only ~7 hours/month active and ~5 posts.
-   **Tech:** Predominantly Desktop (Windows) users.
-   **Social:** Lowest social connectivity with ~79 friends.

**Cluster 3: "The Established Professionals" (Middle-Aged & Moderate)**

-   **Demographics:** Middle-aged (Avg Age: ~40).
-   **Behavior:** Moderate engagement (~19 hours/month).
-   **Tech:** Predominantly Mobile (Android) users.
-   **Loyalty:** Longest account history (Avg Account Age: ~10.3 years).

**Cluster 4: "The Social Connectors" (Young Adults)**

-   **Demographics:** Young adults (Avg Age: ~30).
-   **Behavior:** High engagement (~41 hours/month), but less intense than Cluster 1.
-   **Tech:** Predominantly Mobile (iOS) users.
-   **Social:** Strong social network with ~308 friends.