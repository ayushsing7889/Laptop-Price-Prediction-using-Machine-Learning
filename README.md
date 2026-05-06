# 💻 Laptop Price Analysis & Prediction

A Machine Learning project that analyzes laptop specifications and predicts laptop prices using Python, Data Analysis, Visualization, and Machine Learning techniques.

---

# 🚀 Project Overview

This project focuses on:

* 📊 Data Cleaning & Preprocessing
* 📈 Data Visualization
* 🧠 Feature Engineering
* 🤖 Machine Learning Model Training
* 💰 Laptop Price Prediction

The model predicts laptop prices based on features like RAM, storage, weight, SSD/HDD, and processor type.

---

# 🛠️ Technologies Used

| Technology      | Purpose              |
| --------------- | -------------------- |
| 🐍 Python       | Programming Language |
| 📑 Pandas       | Data Handling        |
| 🔢 NumPy        | Numerical Operations |
| 📊 Matplotlib   | Visualization        |
| 🎨 Seaborn      | Statistical Graphs   |
| 🤖 Scikit-Learn | Machine Learning     |

---

# 📂 Dataset Features

The dataset contains laptop specifications such as:

* 💾 RAM
* ⚖️ Weight
* 💽 HDD
* ⚡ SSD
* 🧠 CPU Type
* 🏷️ Brand
* 💵 Price

---

# 🧹 Data Cleaning

Performed preprocessing tasks like:

* Removing "GB" from RAM
* Removing "kg" from weight
* Converting price columns into numeric values
* Handling missing values
* Removing duplicates

Example:

```python
df["Ram"] = df["Ram"].str.replace("GB","").astype(int)
```

---

# ⚙️ Feature Engineering

Created new useful features like:

* 📦 Total Storage
* 🚀 Performance Score
* 💎 Value Metric
* 🧠 CPU Category
* 💽 SSD/HDD Flags

Example:

```python
df["Performance"] = df["Ram"] * 2 + df["SSD"] * 50
```

---

# 📈 Data Visualization

Used different graphs for analysis:

## 📊 Histogram

Shows data distribution.

## 📉 Scatter Plot

Shows relationship between variables.

Examples:

* RAM vs Price
* Storage vs Price

## 📦 Box Plot

Used to detect outliers.

## 🔥 Heatmap

Shows feature correlation.

---

# 🚨 Outlier Handling

Detected outliers using:

* 📦 Boxplots
* 📐 IQR Method

Formula:

```text
IQR = Q3 - Q1
```

Handled outliers by:

* Removing extreme values
* Capping values
* Log transformation

---

# 🤖 Machine Learning Model

Used:

## 🌲 Random Forest Regressor

Why?

* Good accuracy
* Handles non-linear data
* Reduces overfitting

---

# 🧪 Model Training

Dataset split:

* 📚 Training Data → 80%
* 📝 Testing Data → 20%

Target Variable:

* 💰 Price

Input Features:

* RAM
* Weight
* Storage
* SSD/HDD
* CPU

---

# 📏 Evaluation Metrics

Used:

* 📉 MAE (Mean Absolute Error)
* 📈 R² Score

Lower MAE and higher R² indicate better model performance.

---

# 🎯 Project Outcome

This project successfully:

✅ Cleaned real-world laptop data
✅ Performed exploratory data analysis
✅ Built visual insights using graphs
✅ Predicted laptop prices using Machine Learning

---

# 📁 Project Structure

```text
📦 Laptop-Price-Prediction
 ┣ 📜 laptops.csv
 ┣ 📜 Laptop_Price_Prediction.ipynb
 ┣ 📜 README.md
 ┗ 📜 requirements.txt
```

---

# ▶️ How to Run

## 1️⃣ Clone Repository

```bash
git clone https://github.com/your-username/laptop-price-prediction.git
```

## 2️⃣ Install Libraries

```bash
pip install -r requirements.txt
```

## 3️⃣ Run Jupyter Notebook

```bash
jupyter notebook
```

---

# 📌 Future Improvements

* 🌐 Deploy model using Flask/Streamlit
* 📱 Build web application
* 📊 Improve prediction accuracy
* ☁️ Cloud deployment

---

# 👨‍💻 Author

**Ayush Singh**

---

# ⭐ If you like this project, give it a star on GitHub!
