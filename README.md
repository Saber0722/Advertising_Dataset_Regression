# 📊 Advertising Dataset Regression

This project performs a **simple linear regression** analysis on a classic marketing dataset to understand the impact of TV advertising on product sales. It demonstrates how data-driven insights can be used to optimize marketing strategies using Python and NumPy.

---

## 📚 Dataset Description

The dataset is sourced from [Kaggle - Advertising Dataset](https://www.kaggle.com/datasets/ashydv/advertising-dataset/data) and consists of **advertising budgets across different media channels** and their corresponding **sales figures**.

### 📁 Columns & Units

| Column      | Description                          | Units                   |
|-------------|--------------------------------------|--------------------------|
| `TV`        | Budget spent on TV ads               | Thousands of dollars     |
| `Radio`     | Budget spent on radio ads            | Thousands of dollars     |
| `Newspaper` | Budget spent on newspaper ads        | Thousands of dollars     |
| `Sales`     | Units of product sold                | Thousands of units sold  |

---

## 🧠 Project Objectives

- Analyze the correlation between advertising spend and sales.
- Build a **simple linear regression model** using NumPy.
- Predict product sales based on **TV advertising budget**.
- Visualize relationships using Matplotlib.

---

## 🚀 Getting Started

To run this project locally:

### 1. Clone the repository
```bash
git clone https://github.com/Saber0722/Advertising_Dataset_Regression.git
cd Advertising_Dataset_Regression
```

### 2. Install required packages
```bash
pip install numpy pandas matplotlib
```

### 3. Open the notebook
```bash
jupyter notebook linear_regression.ipynb
```

---

🧪 Methods Used for Regression

This project demonstrates two different approaches to performing linear regression:

    🔢 Closed-form Solution using Pseudo-Inverse

        Implemented manually using NumPy.

        Uses the Moore-Penrose Pseudo-Inverse to handle cases where (XTX) may not be invertible or well-conditioned.

        Formula used:
        θ=(XTX)+XTy

        where (XTX)+ denotes the pseudo-inverse.
        
    📦 Scikit-learn's LinearRegression

        Utilizes the LinearRegression class from sklearn.linear_model.

        A robust and widely-used library method for linear regression.

        Offers features like model evaluation and extension to multiple variables.

This dual approach bridges the gap between theory and practice.

## 📈 Sample Output

After running the linear regression, you might get:

```plaintext
Theta (intercept and slope): [[6.9748], [0.0554]]
Predicted Sales for TV = 230: 19.73
```

This means with **$230,000 spent on TV ads**, the model predicts about **19,730 units** of product will be sold.

---

## 📄 License

This project is licensed under the [MIT License](LICENSE).
