# 📊 Data Visualization Cheat Sheet (Python)

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Seaborn](https://img.shields.io/badge/Seaborn-Statistical%20Plots-green)

A quick reference guide for **data visualization in Python** using **Matplotlib and Seaborn**.

---

# 📌 What is Data Visualization?

Data Visualization is the process of representing data using charts and graphs to:

* Identify patterns
* Detect trends
* Communicate insights
* Support decision making

Common visualization tools in Python:

* Matplotlib
* Seaborn
* Plotly
* Pandas Visualization

---

# ⚙️ Installation

```bash
pip install matplotlib seaborn
```

Import libraries:

```python
import matplotlib.pyplot as plt
import seaborn as sns
import pandas as pd
```

---

# 📈 Line Chart

Used for showing **trends over time**.

```python
import matplotlib.pyplot as plt

x = [1,2,3,4]
y = [10,20,25,30]

plt.plot(x,y)
plt.title("Line Chart Example")
plt.xlabel("X Axis")
plt.ylabel("Y Axis")
plt.show()
```

---

# 📊 Bar Chart

Used for **comparing categories**.

```python
categories = ["A","B","C"]
values = [10,20,15]

plt.bar(categories, values)
plt.title("Bar Chart")
plt.show()
```

---

# 🔵 Scatter Plot

Used to show **relationships between variables**.

```python
x = [1,2,3,4]
y = [10,15,13,17]

plt.scatter(x,y)
plt.title("Scatter Plot")
plt.show()
```

---

# 📉 Histogram

Used for **distribution of data**.

```python
data = [10,20,20,30,40,40,40]

plt.hist(data, bins=5)
plt.title("Histogram")
plt.show()
```

---

# 📦 Box Plot

Shows **data distribution and outliers**.

```python
data = [10,20,30,40,50]

plt.boxplot(data)
plt.title("Box Plot")
plt.show()
```

---

# 🔥 Seaborn Visualization

Seaborn provides **better styling and statistical plots**.

```python
import seaborn as sns
import pandas as pd

data = sns.load_dataset("tips")

sns.scatterplot(x="total_bill", y="tip", data=data)
plt.show()
```

---

# 📊 Heatmap

Used to visualize **correlation between variables**.

```python
import seaborn as sns
import numpy as np

data = np.random.rand(5,5)

sns.heatmap(data)
plt.show()
```

---

# 📊 Pandas Built-in Visualization

```python
df = pd.DataFrame({
    "A":[10,20,30],
    "B":[15,25,35]
})

df.plot(kind="bar")
plt.show()
```

---

# 📊 Common Chart Types

| Chart        | Purpose                        |
| ------------ | ------------------------------ |
| Line Chart   | Trend over time                |
| Bar Chart    | Compare categories             |
| Scatter Plot | Relationship between variables |
| Histogram    | Data distribution              |
| Box Plot     | Distribution & outliers        |
| Heatmap      | Correlation analysis           |

---

# 🚀 Quick Visualization Workflow

```python
import pandas as pd
import matplotlib.pyplot as plt

df = pd.read_csv("data.csv")

df.head()
df.plot(kind="line")

plt.show()
```

---

# 📚 Real-World Use Cases

Data visualization is used in:

* Data Science
* Business Analytics
* Machine Learning
* Financial Analysis
* Dashboard Development

Libraries commonly used together:

* NumPy
* Pandas
* Matplotlib
* Seaborn
* Plotly

---



---

# 📄 License

This project is open-source and available under the **MIT License**.
