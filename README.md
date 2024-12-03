# EV Data Clustering and Analysis

This project involves the cleaning, normalization, and clustering of electric vehicle (EV) data to uncover insights and group similar EV models based on their features. The resulting clusters can help identify trends and groupings in the EV market.

## Table of Contents
- [Overview](#overview)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Features](#features)
- [Results](#results)
- [Future Work](#future-work)
- [License](#license)

---

## Overview

The main goal of this project is to:
1. Clean raw EV data by handling missing values and standardizing columns.
2. Select relevant features such as range, efficiency, and price for clustering.
3. Normalize data and apply **KMeans clustering** to group similar EV models.
4. Save the cleaned and clustered data for further analysis.

---

## Dataset

The dataset includes various features of EVs:
- **Battery Size (kWh)**
- **Top Speed (km/h)**
- **Range (km)**
- **Efficiency (Wh/km)**
- **Fastcharge Speed (km/h)**
- **Price**

### Data Cleaning Steps:
- Missing values in numeric fields were imputed.
- Categorical data, like top speed and fast charge speed, was converted to numeric values.
- Redundant or unnecessary columns were dropped.

---

## Installation

1. Clone the repository or download the project files.
2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```
3. Ensure the dataset is placed in the same directory as the scripts (if not already included).

---

## Usage

1. Run the data cleaning and clustering script:
   ```bash
   python clustering_script.py
   ```
   This script will:
   - Clean the raw data.
   - Normalize selected features.
   - Perform KMeans clustering.

2. The cleaned and clustered data will be saved as `cleaned_and_clustered_ev_data.csv`.

---

## Features

- **Data Cleaning**: Handles missing values and formats inconsistent data.
- **Feature Scaling**: Normalizes data to prepare it for clustering.
- **Clustering**: Groups EV models using KMeans clustering based on:
  - Range (km)
  - Efficiency (Wh/km)
  - Price

---

## Results

- The cleaned dataset is saved as `cleaned_and_clustered_ev_data.csv`.
- Each EV model is assigned a cluster (0, 1, or 2), representing its similarity to other models based on selected features.

---

## Future Work

- Explore more clustering algorithms, like DBSCAN or hierarchical clustering.
- Visualize clusters using dimensionality reduction techniques (e.g., PCA or t-SNE).
- Add more features, such as user reviews or performance metrics, for enhanced clustering.
- Develop a dashboard for interactive exploration of the clustered data.

---

## License

This project is released under the [MIT License](LICENSE).

---

### Author

Developed by Omkar Mishra  
Feel free to reach out for collaboration or feedback!
