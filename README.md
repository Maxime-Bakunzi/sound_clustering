# Clustering Unlabeled Sound Data

## Overview
This project focuses on applying clustering techniques to an unlabeled sound dataset. The primary goal is to extract meaningful features from audio recordings, reduce the high-dimensional feature space to more interpretable dimensions, and then apply clustering algorithms to discover inherent groupings in the data. By comparing different clustering methods, the project highlights the importance of dimensionality reduction in handling complex datasets.

## Project Objectives
- **Feature Extraction:** Extract Mel Spectrogram features from sound files.
- **Visualization:** Attempt to visualize high-dimensional features using scatter and pair plots.
- **Dimensionality Reduction:** Apply PCA and t-SNE to reduce the feature space to 3 dimensions for better visualization and clustering performance.
- **Clustering:** Use K-Means and DBSCAN to cluster the sound data.
- **Performance Evaluation:** Compare clustering outcomes using metrics such as the Silhouette Score and Davies-Bouldin Index.
- **Analysis:** Document and analyze the results to understand why certain methods perform better and the role of dimensionality reduction.

## Dataset
- **Type:** Sound recordings in `.wav` format.
- **Source:** The dataset is provided as part of the assignment (or can be downloaded from the provided link).
- **Structure:** All audio files should be stored in a single directory (e.g., `data/`).

## Project Structure
```
Clustering-Unlabeled-Sound-Data/
│
├── README.md
├── template_clustering_assignment.ipynb    # Jupyter Notebook with complete project code and explanations
├── requirements.txt                        # List of dependencies
└── data/                                   # Folder containing sound (.wav) files
    └── *.wav
```

## Requirements
- Python 3.7 or higher
- Required Python packages:
  - numpy
  - pandas
  - matplotlib
  - seaborn
  - librosa
  - scikit-learn
- **Installation:**  
  Create a virtual environment (optional) and install the dependencies using:
  ```bash
  pip install -r requirements.txt
  ```

## How to Run the Project
1. **Clone the Repository:**  
   Clone or download the project files to your local machine.
2. **Prepare the Dataset:**  
   Place your `.wav` sound files in the `data/` folder.
3. **Update File Paths:**  
   In the Jupyter Notebook (`template_clustering_assignment.ipynb`), update the `data_path` variable to point to your dataset folder.
4. **Launch the Notebook:**  
   Open the Jupyter Notebook:
   ```bash
   jupyter notebook template_clustering_assignment.ipynb
   ```
5. **Execute the Cells:**  
   Run the notebook cells sequentially to perform feature extraction, visualization, dimensionality reduction, clustering, and evaluation.

## Notebook Overview
The notebook is divided into clear sections with explanations preceding each code cell:
1. **Imports and Setup:**  
   Load all necessary libraries.
2. **Data Loading and Feature Extraction:**  
   Load sound files and extract Mel Spectrogram features.
3. **Initial Visualization:**  
   Visualize raw features using scatter and pair plots to highlight challenges with high-dimensional data.
4. **Dimensionality Reduction:**  
   Apply PCA and t-SNE to project the data into a 3D space.
5. **3D Visualization:**  
   Create 3D scatter plots to compare the separability of clusters using PCA and t-SNE.
6. **Clustering Techniques:**  
   Implement K-Means (with optimal cluster determination via the elbow method and silhouette scores) and DBSCAN.
7. **Performance Evaluation:**  
   Evaluate clustering quality using metrics such as Silhouette Score and Davies-Bouldin Index.
8. **Discussion and Final Analysis:**  
   Provide a concise discussion of the results, interpret the findings, and highlight the importance of dimensionality reduction.

## Clustering Methods Used
- **K-Means:**  
  A partition-based algorithm that groups data into a predefined number of clusters by minimizing within-cluster variance.
- **DBSCAN:**  
  A density-based algorithm that clusters data based on the density of points, suitable for discovering clusters of arbitrary shape. Note that DBSCAN may require parameter tuning (e.g., `eps` and `min_samples`).

## Evaluation Metrics
- **Silhouette Score:**  
  Measures how similar an object is to its own cluster compared to other clusters.
- **Davies-Bouldin Index:**  
  Evaluates the average similarity between each cluster and its most similar one, with lower values indicating better clustering.

## Future Improvements
- **Parameter Tuning:**  
  Fine-tune DBSCAN parameters and possibly explore other clustering algorithms.
- **Feature Engineering:**  
  Experiment with additional audio features to improve clustering performance.
- **Advanced Visualization:**  
  Use interactive visualization tools to better explore high-dimensional data.


## Contact
For any questions or further information, please contact:
- **Name:** Maxime Guy Bakunzi
- **Email:** m.bakunzi@alustudent.com

