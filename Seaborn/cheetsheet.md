# 🎨 Seaborn Cheat Sheet

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Visualization-purple)
![Level](https://img.shields.io/badge/Level-Beginner--Intermediate-green)

A quick reference guide for **Seaborn**, a Python library used for **statistical data visualization** built on top of Matplotlib.

---

# 📌 What is Seaborn?

Seaborn is used for creating **beautiful and informative statistical graphics**.

Key advantages:

* Attractive default themes
* Works directly with Pandas DataFrames
* Simplifies complex visualizations
* Ideal for Exploratory Data Analysis (EDA)

---

# ⚙️ Installation

```bash id="wdrutp"
pip install seaborn
```

Import libraries:

```python id="yktwdp"
import seaborn as sns
import matplotlib.pyplot as plt
```

---

# 🎨 Set Style

```python id="7q8y9d"
sns.set_style("darkgrid")
```

Other styles:

```python id="5po6wd"
sns.set_style("whitegrid")
sns.set_style("dark")
sns.set_style("ticks")
```

---

# 🔵 Scatter Plot

Used to show **relationship between variables**.

```python id="dpxkj5"
import seaborn as sns

data = sns.load_dataset("tips")

sns.scatterplot(x="total_bill", y="tip", data=data)

plt.show()
```

Add categories using hue:

```python id="b1my9n"
sns.scatterplot(x="total_bill", y="tip", hue="sex", data=data)
```

---

# 📈 Line Plot

Shows **trends over time**.

```python id="5pmic6"
sns.lineplot(x="total_bill", y="tip", data=data)

plt.show()
```

---

# 📊 Bar Plot

Shows **comparison between categories**.

```python id="h02e2e"
sns.barplot(x="day", y="total_bill", data=data)

plt.show()
```

---

# 📦 Box Plot

Shows **distribution and outliers**.

```python id="y5h7sy"
sns.boxplot(x="day", y="total_bill", data=data)

plt.show()
```

---

# 📉 Histogram

Shows **data distribution**.

```python id="82yecq"
sns.histplot(data["total_bill"])

plt.show()
```

---

# 🔥 Heatmap

Used for **correlation analysis**.

```python id="7v09zn"
corr = data.corr()

sns.heatmap(corr, annot=True)

plt.show()
```

---

# 📊 Pair Plot

Shows **relationships between all numeric variables**.

```python id="0lystz"
sns.pairplot(data)
```

---

# 🎯 Count Plot

Shows **frequency of categories**.

```python id="vyyduf"
sns.countplot(x="day", data=data)

plt.show()
```

---

# 🎨 Customize Plot

Add title:

```python id="42y3g1"
plt.title("Seaborn Chart")
```

Change figure size:

```python id="kjfpxt"
plt.figure(figsize=(8,5))
```

---

# 📊 Common Seaborn Plots

| Plot        | Purpose                         |
| ----------- | ------------------------------- |
| scatterplot | Relationship between variables  |
| lineplot    | Trends over time                |
| barplot     | Category comparison             |
| boxplot     | Distribution and outliers       |
| histplot    | Data distribution               |
| heatmap     | Correlation matrix              |
| pairplot    | Relationships between variables |

---

# 🚀 Quick Reference

```python id="sdypnf"
import seaborn as sns
import matplotlib.pyplot as plt

data = sns.load_dataset("tips")

sns.scatterplot(x="total_bill", y="tip", data=data)
sns.barplot(x="day", y="total_bill", data=data)
sns.boxplot(x="day", y="total_bill", data=data)
sns.histplot(data["total_bill"])

plt.show()
```

---

# 📚 Use Cases

Seaborn is commonly used for:

* Exploratory Data Analysis (EDA)
* Statistical visualization
* Data science projects
* Machine learning analysis

Works well with:

* Pandas
* NumPy
* Matplotlib

---

# ⭐ Contribute

If you find this cheat sheet helpful, consider **starring the repository** and contributing improvements.

---

# 📄 License

This project is open-source and available under the **MIT License**.
