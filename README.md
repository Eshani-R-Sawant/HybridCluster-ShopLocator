 HybridCluster ShopLocator
A Hybrid Clustering–Powered Market Segmentation & Retail Location Intelligence Tool

Using Geospatial, Demographic & Business Data to Identify High-Value Shop Locations in MMR

<p align="center"> <img src="https://img.shields.io/badge/Python-3.9+-blue?style=flat-square"/> <img src="https://img.shields.io/badge/Clustering-HDBSCAN%20%7C%20SCHC%20%7C%20KMeans-orange?style=flat-square"/> <img src="https://img.shields.io/badge/GeoData-QGIS%20%7C%20GeoPandas-green?style=flat-square"/> <img src="https://img.shields.io/badge/Model-RandomForestClassifier-yellow?style=flat-square"/> </p>
 Overview

HybridCluster ShopLocator is a hybrid clustering–based retail market segmentation and shop location evaluation system designed for the Mumbai Metropolitan Region (MMR).

It integrates:

Geospatial data (lat/lon, distance to hubs)

Demographics (population, literacy, worker ratios)

Business features (shop category, revenue)

to generate meaningful and geographically contiguous market clusters, helping retailers answer:

“Where should I open my shop for maximum success?”

The system leverages SCHC, Gower+HDBSCAN, Spectral, and K-Means, with a predictive Random Forest model to classify new locations.

<img width="653" height="350" alt="image" src="https://github.com/user-attachments/assets/706945aa-9a41-4a71-aa3c-e93310d0d38d" />



⚙️ Tech Stack
Languages & Frameworks

Python 3.9+

Libraries Used

Data Processing: pandas, geopandas

Clustering: scikit-learn, HDBSCAN, kmodes

Preprocessing: StandardScaler, OneHotEncoder, PCA

Modeling: RandomForestClassifier

Visualization: matplotlib, seaborn

Project Files
File Name	Description
Final_dataset.csv	Cleaned dataset used for initial model training
final_dataset_engineered_multihub.csv	Feature-engineered dataset for EDA
outputclustering.csv	Cluster output after model execution
hybrid_clustering.py	Main Python code for hybrid clustering pipeline
How to Run
1️⃣ Install Dependencies
pip install pandas geopandas scikit-learn hdbscan kmodes matplotlib seaborn

2️⃣ Load the Notebook or Python Script

Open either the .ipynb or .py file in Jupyter Notebook, VS Code, or PyCharm.

3️⃣ Load Dataset

Make sure Final_dataset.csv is in the same directory.

4️⃣ Run the Pipeline

Execute the cells step-by-step or use “Run All”.

 Outputs Generated

Clustered datasets

🗺 GeoSpatial cluster maps

 Validation plots

Market Segment Prediction via Random Forest

📊 Model Performance
Clustering Comparison
Model	Silhouette	DB Index	CH Index
SCHC	0.5066	0.6244	491.57
Gower + HDBSCAN	0.420	1.068	1709.82
Spectral Clustering	0.533 (Best)	0.569 (Best)	544.88
KMeans	0.398	1.051	1529.13
 Market Segment Predictor

A RandomForestClassifier predicts the market segment of any new shop, based on:

Shop category

Expected revenue

Automatically enriched demographic & geospatial attributes

Helps shop owners evaluate new retail locations quickly.

Future Scope

🇮🇳 Extend project to pan-India retail segmentation

🛰 Integrate Google Places API for real-time competition detection

☁ Deploy as a web application with interactive map

📱 Build Android app for shop owners

🤖 Add LLM-based recommendations (e.g., “best shop type for this area”)

👥 Authors

Eshani Ravindra Sawant

Parth Pitrubhakta

