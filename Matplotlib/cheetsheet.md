# 📊 Matplotlib Cheat Sheet

![Python](https://img.shields.io/badge/Python-3.x-blue?logo=python)
![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-orange)
![Level](https://img.shields.io/badge/Level-Beginner--Intermediate-green)

A quick reference guide for **Matplotlib**, the most widely used Python library for **data visualization and plotting**.

---

# 📌 What is Matplotlib?

Matplotlib is a Python library used to create:

* Line charts
* Bar charts
* Scatter plots
* Histograms
* Box plots
* Subplots and dashboards

It is widely used in **data science, machine learning, and analytics**.

---

# ⚙️ Installation

```bash id="5tnyox"
pip install matplotlib
```

Import library:

```python id="5rkn6j"
import matplotlib.pyplot as plt
```

---

# 📈 Line Plot

Used for showing **trends over time**.

```python id="2q07of"
import matplotlib.pyplot as plt

x = [1,2,3,4]
y = [10,20,30,40]

plt.plot(x,y)
plt.title("Line Chart")
plt.xlabel("X Axis")
plt.ylabel("Y Axis")

plt.show()
```

---

# 📊 Bar Chart

Used to **compare categories**.

```python id="x3vzn3"
categories = ["A","B","C"]
values = [10,20,15]

plt.bar(categories, values)
plt.title("Bar Chart")

plt.show()
```

---

# 🔵 Scatter Plot

Shows **relationship between two variables**.

```python id="i4hgsf"
x = [1,2,3,4]
y = [10,15,13,17]

plt.scatter(x,y)

plt.title("Scatter Plot")
plt.show()
```

---

# 📉 Histogram

Shows **data distribution**.

```python id="jqhr01"
data = [10,20,20,30,40,40,40]

plt.hist(data, bins=5)

plt.title("Histogram")
plt.show()
```

---

# 📦 Box Plot

Shows **data distribution and outliers**.

```python id="w5s9af"
data = [10,20,30,40,50]

plt.boxplot(data)

plt.title("Box Plot")
plt.show()
```

---

# 🎨 Styling Plots

Add grid:

```python id="c1rq0i"
plt.grid(True)
```

Change color:

```python id="yyoqde"
plt.plot(x,y,color="red")
```

Add legend:

```python id="nyed45"
plt.plot(x,y,label="Sales")

plt.legend()
```

---

# 📊 Multiple Plots (Subplots)

```python id="gxb2it"
import matplotlib.pyplot as plt

x = [1,2,3]
y = [10,20,30]

plt.subplot(1,2,1)
plt.plot(x,y)

plt.subplot(1,2,2)
plt.bar(x,y)

plt.show()
```

---

# 💾 Save Plot

Save visualization as image.

```python id="a3h0ob"
plt.savefig("chart.png")
```

---

# 📊 Common Plot Types

| Plot         | Purpose                        |
| ------------ | ------------------------------ |
| Line Plot    | Trend over time                |
| Bar Chart    | Compare categories             |
| Scatter Plot | Relationship between variables |
| Histogram    | Data distribution              |
| Box Plot     | Outliers & spread              |

---

# 🚀 Quick Reference

```python id="31zdkw"
import matplotlib.pyplot as plt

plt.plot(x,y)
plt.bar(x,y)
plt.scatter(x,y)
plt.hist(data)

plt.title("Title")
plt.xlabel("X Label")
plt.ylabel("Y Label")

plt.show()
```

---

# 📚 Use Cases

Matplotlib is used in:

* Data Science
* Machine Learning
* Financial analysis
* Scientific computing
* Data dashboards

It works well with:

* NumPy
* Pandas
* Seaborn

---


