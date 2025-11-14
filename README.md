# Telecommunications Customer Churn Prediction

This repository contains the source code and resources for the CSCE 5380 Data Mining final project by Group 3. The project focuses on identifying key patterns driving customer churn and developing a robust predictive model to identify at-risk customers.

The analysis employs a hybrid data mining approach, combining unsupervised learning (K-Means Clustering, Association Rule Mining) for pattern discovery with supervised learning (Logistic Regression, Decision Trees, SVM) for prediction.

---

## Repository Contents

*   `Customer_Churn_Analysis.ipynb`: The main Jupyter Notebook containing all the code for data preprocessing, data mining, model training, and evaluation.
*   `Telco-Customer-Churn.csv`: The dataset used for this project.
*   `requirements.txt`: A list of required Python libraries for running the notebook in a local environment.
*   `README.md`: This file, providing setup and execution instructions.

---

## Requirements

*   Python 3.8+
*   Jupyter Notebook or access to Google Colab.
*   Required Python libraries are listed in `requirements.txt`.

---

## Setup and Execution Instructions

There are two recommended ways to run this project: using Google Colab (easiest) or in a local environment.

### Option 1: Running in Google Colab (Recommended)

This is the simplest method as most libraries are pre-installed and no local setup is required.

1.  **Open Google Colab:** Go to [colab.research.google.com](https://colab.research.google.com).
2.  **Upload the Notebook:** Click on `File -> Upload notebook` and select the `Customer_Churn_Analysis.ipynb` file from this repository.
3.  **Upload the Dataset:** In the Colab interface, open the "Files" tab on the left sidebar. Click the "Upload to session storage" button and select the `Telco-Customer-Churn.csv` file.
4.  **Install `mlxtend` (if needed):** The `mlxtend` library for Association Rule Mining may not be pre-installed. Run the following command in a code cell at the top of the notebook:
    ```python
    !pip install mlxtend
    ```
5.  **Run the Notebook:** Click on `Runtime -> Run all`. The notebook will execute from top to bottom, generating all outputs and visualizations.

### Option 2: Running in a Local Environment

This method provides more control but requires a local Python installation.

1.  **Clone the Repository:**
    ```bash
    git clone <your-repository-url>
    cd <your-repository-folder>
    ```
2.  **Create a Virtual Environment (Recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```
3.  **Install Required Libraries:**
    ```bash
    pip install -r requirements.txt
    ```
4.  **Launch Jupyter:**
    ```bash
    jupyter notebook
    ```
5.  **Run the Notebook:** Open the `Customer_Churn_Analysis.ipynb` file in Jupyter. Ensure the `Telco-Customer-Churn.csv` file is in the same directory. Click on `Kernel -> Restart & Run All`.

---

## Summary of Findings

The analysis successfully identified a "High-Risk Newcomer" segment (low tenure, high monthly bills) with a **47% churn rate**. The final predictive model, a tuned Logistic Regression, achieved a statistically significant **AUC of 0.841**, proving to be the most effective predictor. The key drivers of churn were found to be Month-to-Month contracts and Fiber Optic service.

### Data Source

The dataset is provided in this repository. The original source is the "Telco Customer Churn" dataset from Kaggle, available at:
[https://www.kaggle.com/datasets/blastchar/telco-customer-churn](https://www.kaggle.com/datasets/blastchar/telco-customer-churn)

---

## Team Members (Group 3)

*   Shiva Sayi Shesshank Mamidi – 11752768
*   Abhiram Reddy Pudi – 11817072
*   Ramanaji Boggarapu – 11718646
*   Sai Kumar Ramisetti – 11822974
