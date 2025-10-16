# PRODIGY_DS_03
Bank Marketing Decision Tree Classifier


Bank Marketing Decision Tree Classifier

Overview

This project implements a Decision Tree Classifier to predict whether a customer will subscribe to a term deposit based on their demographic and behavioral data. The dataset used is the Bank Marketing dataset from the UCI Machine Learning Repository. The project is developed in a Jupyter Notebook using Python and includes data loading, preprocessing, model training, evaluation, and comparison of Decision Tree models using Gini and Entropy criteria.

The goal is to accurately predict customer subscription to a term deposit using features like age, job, marital status, education, campaign contacts, and economic indicators.

Dataset

The dataset is the Bank Marketing dataset (bank-additional-full.csv), containing 41,188 records and 21 columns:





Demographic Features: age, job, marital, education



Behavioral Features: default, housing, loan, contact, month, day_of_week, duration, campaign, pdays, previous, poutcome



Economic Indicators: emp.var.rate, cons.price.idx, cons.conf.idx, euribor3m, nr.employed



Target Variable: y (binary: "yes" for subscription, "no" otherwise)

Source: UCI Machine Learning Repository - Bank Marketing Dataset



Project Structure





Decision_Tree_Classifier.ipynb: Jupyter Notebook with the complete implementation, including:





Data loading and preprocessing



Decision Tree Classifier training with Gini and Entropy criteria



Model evaluation using accuracy, ROC curve, and AUC



Performance comparison of Gini and Entropy models



README.md: This file, providing project overview and instructions.

Prerequisites

The following Python libraries are required:





pandas



numpy



scikit-learn



matplotlib



seaborn



plotly

Install them using:

pip install pandas numpy scikit-learn matplotlib seaborn plotly

How to Run





Download the Dataset:





Download bank-additional-full.csv from the UCI Machine Learning Repository.



Place it in the project directory or update the file path in the notebook.



Set Up Environment:





Open Decision_Tree_Classifier.ipynb in Jupyter Notebook, JupyterLab, or Google Colab.



For Google Colab, mount your Google Drive to access the dataset (as shown in the notebook).



Run the Notebook:





Execute all cells in the notebook.



Ensure the dataset path in pd.read_csv is correct.



The notebook will:





Load and preprocess the dataset



Train Decision Tree models with Gini and Entropy criteria



Evaluate performance with accuracy, ROC curve, and AUC



Display results and conclusions



Expected Output:





Training and testing accuracies of ~93–94% for both Gini and Entropy models.



Visualizations (e.g., decision tree plot, ROC curve) if enabled.



Conclusion comparing Gini and Entropy, with Gini preferred for better recall.

Results





Model Performance:





Both Gini and Entropy models achieve ~93–94% accuracy on training and testing datasets, indicating good generalization.



Gini Criterion: Slightly higher testing accuracy and recall for the positive class ("yes"), making it more effective for identifying subscribers.



Entropy Criterion: Fewer false positives but more false negatives, indicating a conservative approach.



Key Insight: The Gini-based model is recommended for its balanced accuracy and recall, ideal for targeting potential subscribers.

License

This project is licensed under the MIT License.

Acknowledgments





Dataset provided by the UCI Machine Learning Repository.



Built with Python, Scikit-learn, Pandas, and visualization libraries.

Contact

For questions or feedback, open an issue on this repository or contact [Kunal Patel/kunalpatel1538@gmail.com/https://github.com/Kunalpatel-08].



Open in Colab: Click here to run the notebook in Google Colab
