# Laptop Pricing Analysis

## 📌 Project Overview
This project explores the factors influencing laptop prices using data science and machine learning techniques. The dataset contains various specifications of laptops, such as RAM, CPU frequency, GPU, and storage, which are analyzed to predict laptop prices.

## 📊 Features & Analysis
### 1. **Data Preprocessing**
- **Handling Missing Values**: Replaced missing values with mode or mean depending on the feature.
- **Data Type Conversion**: Ensured all numerical features were converted to float for accurate calculations.
- **Feature Engineering**: Created new features such as price bins and performance index.

### 2. **Exploratory Data Analysis (EDA)**
- **Visualizations**: Used histograms, scatter plots, and box plots to understand feature distributions.
- **Feature Correlation**:
  - **RAM_GB**: Strongest positive correlation with price (**0.549**).
  - **CPU_frequency**: Moderate positive correlation (**0.366**).
  - **GPU and Storage**: Significant impact on price (**0.288 & 0.243**, respectively).
  - **Weight & Screen Size**: Low correlation with price, indicating minimal effect.

### 3. **Correlation Analysis & Key Insights**
- **Pearson Correlation** was used to find relationships between features and price.
- **Significant Features**: RAM, CPU cores, SSD storage, GPU, and OS.
- **Low Impact Features**: Weight and screen size showed a weak relationship with price.

### 4. **Machine Learning Models**
- **Single Linear Regression**:
  - **R² Score**: **0.134** (Weak correlation)
  - **MSE**: **284,583** (High error, suggesting a poor fit)
- **Multiple Linear Regression**:
  - **R² Score**: **0.508** (Better fit)
  - **MSE**: **161,680** (Lower error, significant improvement)
- **Ridge Regression** (Hyperparameter tuning with alpha values from 0.001 to 1)
  - Provided better regularization to prevent overfitting.

### 5. **Performance Evaluation & Model Comparison**
- **Multiple Linear Regression outperformed Single Linear Regression**, achieving a significantly higher R² value and lower MSE.
- **Feature importance ranking**:
  1. **RAM** (0.549 correlation)
  2. **CPU Cores & Frequency** (0.459 & 0.366 correlation)
  3. **Storage SSD** (0.243 correlation)
  4. **GPU & OS** (0.288 & -0.221 correlation)
- **Ridge Regression further optimized the model for better stability.**

## 📁 Files in Repository
- `Laptops Pricing.ipynb` - Jupyter Notebook containing all code and analysis.
- `data/` - (Optional) Folder containing dataset files.
- `README.md` - This file, providing an overview of the project.

## 🛠️ Installation & Setup
1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/laptop-pricing-analysis.git
   cd laptop-pricing-analysis
   ```
2. **Install required libraries**:
   ```bash
   pip install -r requirements.txt
   ```
   *(If a requirements.txt file is needed, generate it using `pip freeze > requirements.txt`.)*
3. **Run the Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

## 📈 Results & Key Findings
- **Multiple Linear Regression performed better than Single Linear Regression**, achieving an **R² of 0.508** and a **lower MSE**.
- **RAM, CPU frequency, SSD storage, CPU cores, OS, GPU, and Category are the most significant predictors of price.**
- Ridge regression was used for further tuning and performance improvement.

## 🔗 Contributing
Feel free to fork the repository, raise issues, or contribute improvements!

## 🐜 License
This project is open-source and available under the **MIT License**.

🚀 Happy Coding! 😊
