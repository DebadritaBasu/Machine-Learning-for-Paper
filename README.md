# Machine-Learning-for-Paper
CONTENT:This repository contains two notebooks along with demo data files inside directory named ml_data, used for Machine Learning analysis in paper:

## Prerequisites:
1) Data files for Input for first notebook (RandomForest+K-means.ipynb) are:
   ## saltbridge-tbcol.csv, saltbridge-tb2rr.csv, saltbridge-tbnzo.csv, saltbridge-tb6nl.csv, saltbridge-tbapo.csv
   ## Format: <feature1> ,<feature2> ,..... <featureN> , <label>
3) Data file for Input for second notebook (feature_importances_to_residue_importances.ipynb) is:
   ## feature_importances-processed.csv
   ## Format: <Residue1> ,<Residue2>, <Importance>
# versions of python and python packages used:
1. python 3.9.12 
2. scikit-learn Version: 1.3.0
3. pandas Version: 1.4.2
4. numpy Version: 1.25.2
5. matplotlib Version: 3.5.1
6. scipy Version: 1.11.1
7. seaborn Version: 0.11.2


## Usage:
1. Clone the repository.
2. Update the data_directory variable to point to the directory where your CSV files are stored.
   ## Here at the starting of both the scripts a line is there in the code:
   data_directory = 'C:/Users/HP/Downloads/Machine-Learning-for-Paper-main/Machine-Learning-for-Paper-main/ml_data/'
    ## Remember to Change the path directory with your path to data directory. Which would be something like "your/path/Machine-Learning-for-Paper/ml_data"
3. Run the scripts

## 1)RandomForest+K-means.ipynb
## Motive: Generate a Random Forest model fitted to the data provided, PCA, Projection on PC1-vs-PC2, Clustering, Feature Importance Generation
Tasks:
- Data Preparation: Aligns data, handles missing values, and saves a new CSV file.
- Machine Learning: Uses Random Forest Classifier for classification tasks.
- Feature Importance: Calculates and visualizes feature importances.
- Feature Selection and Dimensionality Reduction: Selects important features and applies PCA.
- Clustering: Applies K-Means clustering and visualizes clusters.
- Data Visualization: Generates colored scatter plots with legend and convex hulls.


## 2)feature_importances_to_residue_importances.ipynb
## Motive : Residue Importance Calculator
Tasks:
- Loads the data into a Pandas DataFrame.
- Identifies unique residues.
- Calculates cumulative importance for each residue.
- Sorts residues by importance.
- Saves the sorted data to a new CSV file.
- Provides a confirmation message.



