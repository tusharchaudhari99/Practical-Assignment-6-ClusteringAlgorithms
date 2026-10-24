:: {align="center"}
# Practical Assignment 6: ClusteringAlgorithms

### Customer Segmentation Using Unsupervised Machine Learning

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-Clustering-orange?logo=scikitlearn&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter&logoColor=white)
![Status](https://img.shields.io/badge/Project-Academic%20Assignment-blue)
:::📌 Project Overview
This practical assignment applies and compares three unsupervised
machine learning algorithms to the Mall Customers dataset. Customers
are grouped using their Annual Income (k$) and Spending Score
(1-100).

The project covers data inspection, cleaning, exploratory data analysis
(EDA), feature scaling, clustering, evaluation, visualization,
customer-segment profiling, and exporting results.
Goal: Explore customer groups and compare the strengths of
K-Means, Hierarchical Clustering, and DBSCAN.

🎯 Objectives
- Understand and prepare the Mall Customers dataset.
- Inspect missing values, duplicates, data types, and summary
  statistics.
- Perform EDA and visualize relationships between selected features.
- Standardize features before applying clustering algorithms.
- Apply K-Means, Agglomerative (Hierarchical) Clustering, and DBSCAN.
- Compare cluster quality with Silhouette Score and Davies--Bouldin
  Index.
- Visualize clusters and summarize customer segments.
- Export cluster labels and comparison metrics to CSV files.
🗂️ Dataset
Dataset file: Mall_Customers.csv

The standard dataset contains customer information such as:

  Column                     Description
  CustomerID               Customer identifier
  Gender                   Customer gender
  Age                      Customer age
  Annual Income (k$)       Annual income in thousands of dollars
  Spending Score (1-100)   Spending score on a scale of 1 to 100
Features used for clustering
- Annual Income (k$)
- Spending Score (1-100)
The notebook uses these two numeric features as clustering inputs. Other
available columns may be used for understanding the customer groups
after clustering.
🧠 Algorithms
<details>
<summary>
<strong>{=html}1. K-Means Clustering</strong>{=html}
</summary>
K-Means groups observations into k clusters by assigning each customer
to the nearest cluster centroid. Candidate values of k are compared
using the Elbow Method (inertia) and Silhouette Score.
</details>
<details>
<summary>
<strong>{=html}2. Hierarchical (Agglomerative)
Clustering</strong>{=html}
</summary>
Agglomerative clustering starts with individual observations and merges
groups step by step. This notebook uses Ward linkage and the selected
number of clusters.
</details>
<details>
<summary>
<strong>{=html}3. DBSCAN</strong>{=html}
</summary>
DBSCAN forms clusters based on density and can identify noise points.
The notebook tests multiple eps values with min_samples = 5, then
evaluates the number of clusters, noise points, and clustering metrics.
</details>
🔄 Project Workflow
Load Dataset
     ↓
Inspect and Clean Data
     ↓
Exploratory Data Analysis (EDA)
     ↓
Select Income and Spending Features
     ↓
Standardize Features
     ↓
Apply Clustering Algorithms
     ├── K-Means
     ├── Hierarchical Clustering
     └── DBSCAN
     ↓
Evaluate and Compare Results
     ↓
Visualize Clusters and Profile Segments
     ↓
Export CSV Results
📊 Evaluation Metrics
  Metric                  What it indicates       Preferred direction
  Silhouette Score        How well observations   Higher
                          fit within their
                          clusters compared with
                          other clusters          

  Davies--Bouldin Index   Cluster compactness and Lower
                          separation              

  Number of clusters      How many groups the     Interpret in context
                          algorithm found         

  DBSCAN noise points     Observations DBSCAN     Interpret in context
                          marked as outliers
                      (-1)                  
For DBSCAN, Silhouette Score and Davies--Bouldin Index are calculated on
non-noise observations when at least two clusters remain.
🛠️ Tools and Technologies
- Language: Python
- Environment: Jupyter Notebook / JupyterLab
- Data handling: Pandas, NumPy
- Visualization: Matplotlib, Seaborn
- Machine learning: Scikit-learn
⚙️ Installation
Install the required libraries:
pip install numpy pandas matplotlib seaborn scikit-learn jupyter
▶️ How to Run
1. Clone or download this repository.
2. Put Mall_Customers.csv in the same folder as the notebook.
3. Install the packages listed above.
4. Launch Jupyter:
   jupyter notebook
5. Open the assignment notebook.
6. Run the cells from top to bottom.
Note: The notebook uses Jupyter's display() function, so run it
in Jupyter Notebook or JupyterLab for the intended output and charts.

📁 Output Files
The notebook exports these files after a successful run:
  Output file                                  Description
  Mall_Customer_Cluster_Labels.csv           Customer data with K-Means,
                                               Hierarchical, and DBSCAN cluster
                                               labels

  Mall_Clustering_Algorithm_Comparison.csv   Comparison table containing cluster
                                               counts, noise statistics, and
                                           evaluation metrics
The notebook also displays EDA charts, K-Means selection plots, DBSCAN
tuning results, cluster visualizations, customer-segment summaries, and
algorithm comparison metrics.
📂 Suggested Repository Structure
Practical-Assignment-6-ClusteringAlgorithms/
├── Mall_Customer_Clustering_Best_Notebook_Checked(2).ipynb
├── Mall_Customers.csv
├── README.md
├── Mall_Customer_Cluster_Labels.csv            # generated by the notebook
└── Mall_Clustering_Algorithm_Comparison.csv    # generated by the notebook
👤 Author
Tushar Vijay Chaudhari
  Detail                              Information
  Institution                         MIT Academy of Engineering (MIT
                                      AOE), Alandi, Pune

  Department                          Electronics and Telecommunication
                                      Engineering (ENTC)

  Assignment                          Practical Assignment 6 ---
                                      Clustering Algorithms

  Technologies                        Python, Pandas, NumPy, Matplotlib,
                                  Seaborn, Scikit-learn
🏁 Conclusion
This assignment demonstrates how centroid-based, hierarchical, and
density-based clustering methods can discover customer groups using
annual income and spending score. The visualizations and evaluation
metrics help compare the algorithms and interpret the segments they
identify.
::: {align="center"}
**Practical Assignment 6: ClusteringAlgorithms**\
*Academic machine learning project*
:::
