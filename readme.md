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

# 📊 Python Data Visualization Libraries Comparison

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Visualization](https://img.shields.io/badge/Data-Visualization-orange)
![Level](https://img.shields.io/badge/Level-Beginner--Intermediate-green)

This guide explains the differences between the most popular **Python data visualization libraries**:

* Matplotlib
* Seaborn
* Plotly
* Cufflinks

These libraries are commonly used in **data science, machine learning, and analytics workflows**.

---

# 📌 Overview

| Library    | Type                      | Interactivity | Best For                     |
| ---------- | ------------------------- | ------------- | ---------------------------- |
| Matplotlib | Core plotting library     | ❌ No          | Custom visualizations        |
| Seaborn    | Statistical visualization | ❌ No          | Beautiful statistical charts |
| Plotly     | Interactive visualization | ✅ Yes         | Dashboards & web charts      |
| Cufflinks  | Plotly wrapper for Pandas | ✅ Yes         | Quick interactive plots      |

---

# 📈 Matplotlib

Matplotlib is the **foundation plotting library in Python**. Most visualization libraries build on top of it.

### Key Features

* Highly customizable
* Supports many chart types
* Works well with NumPy and Pandas
* Static visualizations

### Example

```python id="t7ynfu"
import matplotlib.pyplot as plt

x = [1,2,3]
y = [10,20,30]

plt.plot(x,y)
plt.title("Line Chart")
plt.show()
```

### Pros

✔ Full control over charts
✔ Highly flexible

### Cons

❌ More code required
❌ Default styling is basic

---

# 🎨 Seaborn

Seaborn is a **high-level visualization library built on Matplotlib** designed for statistical graphics.

### Key Features

* Beautiful default themes
* Statistical plots
* Works directly with Pandas DataFrames

### Example

```python id="93f7vc"
import seaborn as sns
import matplotlib.pyplot as plt

data = sns.load_dataset("tips")

sns.scatterplot(x="total_bill", y="tip", data=data)
plt.show()
```

### Pros

✔ Attractive plots
✔ Less code required

### Cons

❌ Less customization compared to Matplotlib

---

# 🚀 Plotly

Plotly is a **modern interactive visualization library** used for dashboards and web-based analytics.

### Key Features

* Interactive charts
* Hover information
* Zoom and pan
* 3D charts

### Example

```python id="kmbp8h"
import plotly.express as px

df = px.data.iris()

fig = px.scatter(df, x="sepal_width", y="sepal_length")
fig.show()
```

### Pros

✔ Interactive graphs
✔ Modern UI

### Cons

❌ Slightly heavier library

---

# 🔗 Cufflinks

Cufflinks connects **Pandas DataFrames with Plotly** to generate interactive charts easily.

### Key Features

* Simple interactive charts
* Works directly with Pandas
* Uses Plotly backend

### Example

```python id="hh6n31"
import pandas as pd
import cufflinks as cf

cf.go_offline()

df = pd.DataFrame({
    "A":[10,20,30],
    "B":[15,25,35]
})

df.iplot(kind="bar")
```

### Pros

✔ Very easy to use
✔ Interactive charts

### Cons

❌ Less flexibility than Plotly

---

# 📊 Feature Comparison

| Feature         | Matplotlib | Seaborn | Plotly | Cufflinks |
| --------------- | ---------- | ------- | ------ | --------- |
| Customization   | ⭐⭐⭐⭐       | ⭐⭐⭐     | ⭐⭐⭐    | ⭐⭐        |
| Ease of Use     | ⭐⭐         | ⭐⭐⭐⭐    | ⭐⭐⭐    | ⭐⭐⭐⭐      |
| Interactivity   | ❌          | ❌       | ✅      | ✅         |
| Dashboard Ready | ❌          | ❌       | ✅      | ✅         |

---

# 🧠 When to Use Each Library

Use **Matplotlib** when you need **full control over visualization**.

Use **Seaborn** when performing **statistical analysis and exploratory data analysis (EDA)**.

Use **Plotly** when building **interactive dashboards or web applications**.

Use **Cufflinks** when you want **quick interactive charts directly from Pandas DataFrames**.

---

# 🚀 Data Visualization Workflow

A typical data science workflow:

```text id="r2ngaw"
NumPy → Pandas → Seaborn → Plotly
```

Explanation:

* NumPy → numerical computation
* Pandas → data manipulation
* Seaborn → statistical visualization
* Plotly → interactive dashboards

---





---

# 📄 License

This project is open-source and available under the **MIT License**.
