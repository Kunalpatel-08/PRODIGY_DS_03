# 🏦 PRODIGY_DS_03  
### **Bank Marketing Decision Tree Classifier**

---

## 📘 Overview

This project implements a **Decision Tree Classifier** to predict whether a customer will subscribe to a **term deposit** based on their **demographic** and **behavioral data**.  
The dataset used is the **Bank Marketing dataset** from the [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/222/bank+marketing).

The project is built in **Python** using **Jupyter Notebook** and includes:

- Data loading and preprocessing  
- Decision Tree model training using **Gini** and **Entropy** criteria  
- Model evaluation using **Accuracy**, **ROC Curve**, and **AUC**  
- Performance comparison between both criteria  

The goal is to accurately predict customer subscription to a term deposit using features like **age**, **job**, **marital status**, **education**, **campaign contacts**, and **economic indicators**.

---

## 📊 Dataset

**Source:** [UCI Machine Learning Repository - Bank Marketing Dataset](https://archive.ics.uci.edu/dataset/222/bank+marketing)  
**File:** `bank-additional-full.csv`  
**Records:** 41,188  
**Columns:** 21  

### 🔹 Demographic Features
- `age`
- `job`
- `marital`
- `education`

### 🔹 Behavioral Features
- `default`
- `housing`
- `loan`
- `contact`
- `month`
- `day_of_week`
- `duration`
- `campaign`
- `pdays`
- `previous`
- `poutcome`

### 🔹 Economic Indicators
- `emp.var.rate`
- `cons.price.idx`
- `cons.conf.idx`
- `euribor3m`
- `nr.employed`

### 🎯 Target Variable
- `y` → binary classification (`yes` = subscribed, `no` = not subscribed)

---

## 🧱 Project Structure

```
📂 Bank_Marketing_DecisionTree/
│
├── Decision_Tree_Classifier.ipynb    # Complete implementation notebook
├── bank-additional-full.csv           # Dataset (to be downloaded)
└── README.md                          # Project overview and guide
```

---

## ⚙️ Prerequisites

Install the required Python libraries before running the notebook:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn plotly
```

---

## 🚀 How to Run

### 1️⃣ Download the Dataset
- Download `bank-additional-full.csv` from the [UCI Repository](https://archive.ics.uci.edu/dataset/222/bank+marketing).  
- Place it in your project folder or update the file path in the notebook.

### 2️⃣ Set Up the Environment
- Open the notebook `Decision_Tree_Classifier.ipynb` in **Jupyter Notebook**, **JupyterLab**, or **Google Colab**.  
- If using **Google Colab**, mount your Google Drive as shown in the notebook to access the dataset.

### 3️⃣ Execute the Notebook
- Run all cells sequentially.  
- Ensure the dataset path in `pd.read_csv()` is correct.  
- The notebook will:
  - Load and preprocess the dataset  
  - Train models using Gini and Entropy  
  - Evaluate models  
  - Display comparison results and visualizations

---

## 📈 Expected Output

- Training and Testing Accuracy: **~93–94%** for both Gini and Entropy models  
- Model Visualizations:
  - Decision Tree Plot (if enabled)
  - ROC Curve and AUC
- Final Comparison Summary between both models

---

## 🧠 Results and Insights

| Criterion | Training Accuracy | Testing Accuracy | Key Characteristic |
|------------|------------------:|-----------------:|--------------------|
| **Gini**   | ~93.6%            | ~93.3%           | Higher recall for subscribers |
| **Entropy**| ~93.4%            | ~93.2%           | More conservative (fewer false positives) |

### 🔍 Key Insights
- Both models generalize well with consistent train-test accuracy.  
- **Gini Criterion** shows slightly better recall, making it more effective for identifying likely subscribers.  
- **Entropy Criterion** results in fewer false positives but may miss potential subscribers.  

✅ **Recommended Model:** Gini Criterion — for balanced accuracy and recall, ideal for marketing target optimization.

---

## 🪄 Visualizations
- Decision Tree structure (using Graphviz or Plotly)
- ROC Curves for Gini vs Entropy
- Feature importance visualization

---

## 📜 License
This project is licensed under the **MIT License**.

---

## 🙏 Acknowledgments
- Dataset: [UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/222/bank+marketing)  
- Tools used: **Python**, **Scikit-learn**, **Pandas**, **Matplotlib**, **Seaborn**, **Plotly**

---

## 💬 Contact

**Kunal Patel**  
📧 [kunalpatel1538@gmail.com](mailto:kunalpatel1538@gmail.com)  
🌐 [GitHub Profile](https://github.com/Kunalpatel-08)  

---

## ▶️ Open in Google Colab
Click below to run the notebook directly in Google Colab:  
🔗 [**Open in Colab**](https://colab.research.google.com/drive/1gfYtKWvZAqwd8FyxL4cTzd6DuhpaD2NZ#scrollTo=4064b6bb)
