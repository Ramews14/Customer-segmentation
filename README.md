# Customer Segmentation using K-Means Clustering

## Project Description

This project applies **K-Means clustering** to segment customers based on their demographic and behavioral data. Customer segmentation is an important technique in marketing and business, enabling companies to target specific customer groups more effectively by understanding their preferences, spending patterns, and other attributes.

In this project, we perform the following steps:
- Data preprocessing (handling missing values, standardization)
- Apply K-Means clustering to group customers into clusters
- Evaluate the clusters using metrics such as the **silhouette score**
- Visualize the results of the clustering

## Dataset

The dataset consists of customer demographic and behavioral data, including features such as:
- **Age**: The age of the customer
- **Gender**: Male or Female
- **Profession**: The occupation of the customer
- **Spending Score**: A score that ranks customer spending behavior
- **Work Experience**: Years of work experience of the customer
- **Family Size**: The number of family members in the customer's household

## Project Steps

1. **Data Preprocessing**:
    - Handling missing values by imputing or dropping rows/columns with null values.
    - Standardizing the feature values to ensure all variables contribute equally to the K-Means algorithm.

2. **K-Means Clustering**:
    - Used to segment customers into `n` clusters based on their feature similarities.
    - Optimal number of clusters chosen using **elbow method** and **silhouette score**.

3. **Model Evaluation**:
    - Evaluate the clustering quality using the **silhouette score** which measures how well the data points fit within their clusters.
    - A silhouette score of **0.42** was achieved, indicating moderate clustering quality.

4. **Visualization**:
    - Visualizing the clusters in a 2D or 3D space based on principal components or selected feature pairs.

## Installation

To run this project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/customer-segmentation-kmeans.git
    ```

2. Install the required dependencies using `requirements.txt`:
    ```bash
    pip install -r requirements.txt
    ```

3. Run the Python scripts for data preprocessing, clustering, and evaluation:
    ```bash
    python kmeans_clustering.py
    ```

## Usage

- Adjust the number of clusters in the `kmeans_clustering.py` script to explore different customer segmentations.
- Visualize the clusters using the provided visualization scripts.

## Metrics Used

- **Silhouette Score**: Measures the cohesion and separation of clusters. The score ranges from -1 to 1, where 1 indicates well-separated clusters. Our model achieved a score of **0.42**, indicating moderate cluster quality.



