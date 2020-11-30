# Wearable Stress and Affect Recognition

Analysis of the Wearable Stress and Affect Recognition Dataset (WESAD).

A report of this project in IEEE format is provided [here](./report.pdf)

# Dataset

The WESAD dataset can be found on [UCI repository](https://archive.ics.uci.edu/ml/datasets/WESAD+%28Wearable+Stress+and+Affect+Detection%29).

The complete dataset (*2.1GB compressed*, 16.4GB uncompressed) consists of 15 sub-directories corresponding to *15 test subjects*.
Each sub-directory consists of the raw CSV (chest data) and zip file (wrist data) as well as a pickle (.pkl) file containing the
data combined from both the devices.

We convert these pickle files to CSVs for easier handling.

# Usage Instructions

 - Install all the requirements using `pip install -r requirements.txt`.
 - To work on the original dataset, the following has to be followed.
    - Open [`EDA.ipynb`](./notebooks/EDA.ipynb) in jupyter and run cells in till the section titles "Convert data (run only once)"
    - This might take some time as it will convert all the pickle files to CSV files (each of them is 800-1000MB).
    - You can now continue with the EDA notebook or run the other notebooks.
 - Alternatively, if you do not want to run the notebooks on the entire data, we provide a sample of the data [here](https://drive.google.com/file/d/1j5Va94cCim5-56Tp9p8G5WATVvsEXDod/view?usp=sharing)
    - Place the sample in the notebooks directory and adjust the data loading cell to ensure it loads the sample data.

# Files

 - [`EDA.ipynb`](./notebooks/EDA.ipynb): notebook for data exploration and for converting the pickle files to CSV files (see dataset section).
 - [`PCA.ipynb`](./notebooks/PCA.ipynb): notebook for Principal Component Analysis (PCA) in 2 dimensions
 - [`PCA_with_n_3.ipynb`](./notebooks/PCA_with_n_3.ipynb): notebook for PCA in 3 dimensions
 - [`PCA_3_plotly.ipynb`](./notebooks/PCA_3_plotly.ipynb): same as above, but cleaner and includes a 3D plot of the reduced dimensions
 - [`KMeans.ipynb`](./notebooks/KMeans.ipynb): notebook for K-Means clustering
 - [`DBSCAN.ipynb`](./notebooks/DBSCAN.ipynb): notebook for DBSCAN clustering
 - [`Classification.ipynb`](./notebooks/Classification.ipynb): notebook for training and comparing classification models. This was run in Google Colab.
 - [`report.pdf`](./report.pdf): Project report in IEEE format
 - [`graphs`](./graphs): Graphs for data visualisations

# Team members

 - [Samyak Sarnayak](https://github.com/Samyak2)
 - [Pranav Kesavarapu](https://github.com/psiayn)
 - [Abhijit Mohanty](https://github.com/mohantyabhijit074)
 - [Raghav Aggarwal](https://github.com/RaghavAgg0310)

