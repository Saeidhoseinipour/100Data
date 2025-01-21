# 100Data: A Comprehensive Guide to 100 Biostatistics Datasets — Cleaning, Exploration, Modeling, and Visualization

**100Data** is an in-depth project aimed at addressing **complex biostatistics datasets** through a structured workflow of data cleaning, exploratory analysis, and the implementation of **efficient, interpretable machine learning models**. The project centers on **100 challenging datasets**, including gene expression profiles, clinical trial data, and patient demographics, offering a systematic approach to deriving actionable insights from raw data. By employing **streamlined, technical models** such as Random Forests, Logistic Regression, and K-Means clustering, we demonstrate how scalable and reproducible machine learning techniques can be effectively applied to real-world biostatistics challenges.


##  Overview




## Project Structure

The project is organized as follows:

- **`README.md`**: The main documentation file.
- **`notebooks/`**: Contains Jupyter Notebooks for data exploration, model training, and visualization.
  - `DataExplorer.ipynb`
  - `ModelTrainer.ipynb`
  - `ModelVisualizer.ipynb`
- **`src/`**: Contains Python scripts for data cleaning and exploration.
  - `cleaner.py`
  - `explorer.py`

---

### Goal
To provide a step-by-step guide for working with 100 **hardcore biostatistics datasets**, covering:
- **Data Cleaning**
- **Exploratory Data Analysis (EDA)**
- **Short, Technical Machine Learning Models**
- **Visualization**

### Scope
- Focus on **complex datasets** relevant to biostatistics, including gene expression, clinical trials, patient data, and more.
- Use **efficient and interpretable machine learning models** to ensure reproducibility and scalability.
- Compile findings into a **high-quality paper**.


---

## Big Picture of Project Steps



### 1. Data Collection
- Identify 100 **hardcore datasets** relevant to biostatistics.
- Sources: Public repositories (e.g., Kaggle, UCI, NCBI, TCGA), research papers, and synthetic data.
- Organize datasets into categories:
  - **Quantitative Data:** Gene expression, clinical measurements.
  - **Qualitative Data:** Patient demographics, disease classifications.
  - **Time-to-Event Data:** Survival analysis, clinical trials.
  - **Network Data:** Protein-protein interactions, gene networks.



### 2. Data Cleaning and Preparation
- Develop a Python class ([`BioinformaticsDatasetCleaner`](notebooks/BioinformaticsDatasetCleaner.ipynb)) to:
  - Load datasets from various formats (CSV, Excel, JSON, etc.).
  - Handle missing values, duplicates, and outliers.
  - Convert data types and standardize formats.
- Tag datasets with metadata:
  - **Type:** Quantitative, qualitative, time-to-event, etc.
  - **Features:** Column names and descriptions.
  - **Source:** Origin of the dataset.



| Dataset Name          | Type            | Size       | Features                          | Use Case                           | Source       | Challenges                     |
|-----------------------|-----------------|------------|-----------------------------------|------------------------------------|--------------|--------------------------------|
| **Titanic**           | Qualitative     | 891 rows   | Class, Age, Sex, Survived         | Survival analysis                  | Kaggle       | Missing values in Age          |
| **Breast Cancer**     | Quantitative    | 569 rows   | Mean radius, Mean texture, Target | Classification (malignant/benign)  | UCI          | None                           |
| **Iris**              | Quantitative    | 150 rows   | Sepal length, Sepal width, Species| Classification (flower species)    | UCI          | None                           |
| **Diabetes**          | Quantitative    | 442 rows   | Age, BMI, BP, Target              | Regression (disease progression)   | Scikit-learn | None                           |
| **Gene Expression**   | Quantitative    | 100x20     | Gene_1 to Gene_100, Sample        | Gene expression analysis           | Synthetic    | High dimensionality            |
| **Cell Cycle**        | Qualitative     | 50 rows    | Cell, Phase                       | Cell cycle phase classification    | Synthetic    | Small sample size              |
| **Protein Interaction**| Network        | 10x10      | Protein_1 to Protein_10           | Protein-protein interaction analysis| Synthetic    | Sparse interactions            |
| **TCGA BRCA**         | Quantitative    | 100x50     | Gene_1 to Gene_100, Patient       | Cancer subtype classification      | TCGA         | High dimensionality            |
| **Flights**           | Quantitative    | 144 rows   | Year, Month, Passengers           | Time-series analysis               | Seaborn      | None                           |
| **Diamonds**          | Quantitative    | 53,940 rows| Carat, Cut, Color, Price          | Regression (price prediction)      | Seaborn      | Large dataset size             |



### 3. Exploratory Data Analysis (EDA)
- Develop a Python class ([`DataExplorer`](notebooks/DataExplorer.ipynb)) to:
  - Compute descriptive statistics (mean, median, variance, etc.).
  - Visualize data distributions (histograms, box plots, scatter plots).
  - Identify correlations and patterns.
- Generate summary reports for each dataset:
  - Key statistics.
  - Visualizations.
  - Insights and observations.



### 5. Machine Learning Modeling
- Develop a Python class ([`ModelTrainer`](notebooks/ModelTrainer.ipynb)) to:
  - Split data into training and testing sets.
  - Train **short, technical models** based on dataset type:
    - **Classification:** Random Forest, Logistic Regression.
    - **Regression:** Linear Regression, Random Forest Regressor.
    - **Clustering:** K-Means, Hierarchical Clustering.
  - Evaluate models using appropriate metrics:
    - Accuracy, precision, recall (classification).
    - Mean Squared Error, R-squared (regression).
    - Silhouette Score (clustering).

### 6. Model Visualization
- Develop a Python class ([`ModelVisualizer`](notebooks/ModelVisualizer.ipynb)) to:
  - Plot confusion matrices for classification models.
  - Visualize ROC curves and AUC scores.
  - Generate residual plots for regression models.
  - Visualize clusters for unsupervised models.
- Create interactive visualizations using libraries like Plotly or Seaborn.



### 7. Project Integration
- Develop a Python class (`ProjectManager`) to:
  - Integrate all steps into a cohesive workflow.
  - Automate dataset processing, modeling, and visualization.
- Create a user-friendly interface:
  - Allow users to select datasets and apply specific analyses.
  - Generate reports and visualizations on demand.



### 8. Documentation and Reporting
- Document the project:
  - Write a detailed README file.
  - Include instructions for running the code.
  - Provide examples and use cases.
- Generate automated reports:
  - Summarize dataset statistics.
  - Include visualizations and model performance metrics.



### 9. Deployment and Sharing
- Deploy the project as a web application:
  - Use Flask or Streamlit for a user-friendly interface.
  - Host on platforms like Heroku or AWS.
- Share the project:
  - Publish on GitHub with open-source licensing.
  - Write a blog post or tutorial to explain the project.



### 10. High-Quality Paper
- Compile findings into a **high-quality paper**:
  - Include detailed methodology, results, and visualizations.
  - Submit to relevant academic journals or conferences.

---
