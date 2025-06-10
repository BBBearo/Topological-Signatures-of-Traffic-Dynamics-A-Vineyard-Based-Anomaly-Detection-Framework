# Topological Signatures of Traffic Dynamics: A Vineyard-Based Anomaly Detection Framework

This project applies Topological Data Analysis (TDA) techniques to detect anomalous patterns in freeway traffic data using persistent homology and vineyard-based features.

---

## Setup Instructions

### 1. Clone the Repository
```bash
git clone https://github.com/BBBearo/Topological-Signatures-of-Traffic-Dynamics-A-Vineyard-Based-Anomaly-Detection-Framework.git
cd Topological-Signatures-of-Traffic-Dynamics-A-Vineyard-Based-Anomaly-Detection-Framework
```

### 2. Install Dependencies
Make sure you have Python 3.8+ and `pip`. Then run:
```bash
pip install -r requirements.txt
```

---

## Run the Project

### 3. Launch the Notebook
Open the main notebook:
```
project.ipynb
```

### 4. Choose a Location to Analyze
In the notebook, find the section:
```python
location = "805 NB S/O Orange/Olympic"
```
Replace this with any sensor location name found in the provided dataset CSV (located in `./dataset/Caltran/250414model_ready_output_final.csv`).

You can preview available locations using:
```python
pd.read_csv("./dataset/Caltran/250414model_ready_output_final.csv")["location"].unique()
```

---

## Outputs

The notebook will generate:

- Topological features (Persistence Images)
- Entropy-based complexity scores
- t-SNE anomaly visualizations
- Supervised/unsupervised anomaly predictions

All results will be saved as CSV and PNG files.

---

## Author
Developed by [@BBBearo](https://github.com/BBBearo)
