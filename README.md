# Unsupervised Clustering on Market Data

## Author
**Mohd Nasar Siddiqui (220661)**

## Overview
This project explores unsupervised learning techniques on high-frequency trading data. It leverages engineered market microstructure features and applies dimensionality reduction via autoencoders, followed by clustering using Gaussian Mixture Models (GMM) and HDBSCAN.

## Dataset
The data used includes:
- `aggTrade.txt` files: Combined into a single `aggTrade.csv`.
- `depth20_1000ms.txt` files: Combined into a single `depth20_1000ms.csv`.
Dataset link -> https://drive.google.com/drive/folders/1gFLwPLTE0nUN-MHoOn5u_1yrlbpI3Fst

## Pipeline

1. **Data Extraction**: 
   - Merged raw text files into consolidated CSVs for processing, and to capture non-linear patterns.

2. **Feature Engineering**: 
   - Includes spread, microprice, order book imbalance, cumulative quantities, volatility, VWAP, slopes, and time-based features.

3. **Dimensionality Reduction**:
   - PCA is used for Dimensionality Reduction

4. **Feature Extraction**:
   - Autoencoder is used to extract a compressed latent representation of the feature set.

5. **Clustering**:
   - GMM for probabilistic clustering.
   - HDBSCAN for density-based clustering without needing to predefine cluster count.

## Results
Clusters were visualized in 2D latent space and correspond to distinct trading patterns or market regimes.

## Requirements
- Python 3.x
- pandas, numpy, sklearn, tensorflow/keras, matplotlib, seaborn, hdbscan

## How to Run
1. Save the aggTrade and depth20_1000ms folders in your google drive.
2. Install all the neccessary python libraries listed above.
3. Execute the code.

## Credits and References
The dataset used is provided by RozReturns

## License
Enjoy !!!
