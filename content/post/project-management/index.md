---
title: ✅ Manage your projects
summary: Easily manage your projects - create ideation mind maps, Gantt charts, todo lists, and more!
date: 2023-10-23
authors:
  - admin
tags:
  - Hugo Blox
  - Markdown
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com)'
---

## Weekly Projects Update

### Lab Project 1: Simulation Modeling in Python

**Objective:**
The goal of this lab was to familiarize myself with simulation modeling using Python and to explore key programming techniques for data generation and visualization. Over the course of this project, I delved into basic data types, data input/output commands, and statistical methods for handling random data.

---

#### Task 1: Generating a Matrix of Random Numbers

**Description:**
In this task, I created a matrix with 10 rows and 2 columns, where each element is filled with random numbers uniformly distributed between two values. The purpose of this exercise was to explore how random values can be generated and visualized as points on a graph.

**Code Example:**
```python
import numpy as np
import matplotlib.pyplot as plt

# Create a 10x2 matrix of random numbers
m = 10  
n = 2  
mu = 0     
sigma = 10  
matrix = np.random.uniform(mu, sigma, (m, n))

# Print the matrix
print(matrix)

# Visualize the data as a scatter plot
plt.figure(figsize=(10, 6))
plt.scatter(matrix[:, 0], matrix[:, 1], alpha=0.8, color="red", label="Matrix Points")
plt.xlim(0,12)
plt.ylim(0,12)
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.title("Uniformly Distributed Random Numbers")
plt.grid(True)
plt.show()
```

**Outcome:**
I generated a 10x2 matrix of random values and visualized these points on a scatter plot. The uniform distribution helped ensure that values were spread out evenly across the given range. The result was a clear visualization, which demonstrated the randomness and distribution of data points.

---

#### Task 2: Generating and Analyzing 1000 Random Numbers

**Description:**
This task involved generating 1000 random numbers from a normal distribution, calculating their mean and variance, and visualizing the data using a histogram.

**Code Example:**
```python
# Generate 1000 random numbers with a normal distribution
exp_sample_1000 = np.random.normal(scale=1, size=1000)

# Calculate the mean and variance
E = sum(exp_sample_1000)/len(exp_sample_1000)
Var = np.var(exp_sample_1000)

# Visualize the histogram
plt.figure(figsize=(10, 6))
plt.hist(exp_sample_1000, bins=30, density=True, alpha=0.8, color="skyblue", label="Sample Histogram")
plt.axvline(E, color='r', linewidth=3, label='Mean')
plt.axvline(E + Var, color='g', linewidth=2, label="Mean + Standard Deviation")
plt.axvline(E - Var, color='g', linewidth=2, label="Mean - Standard Deviation")
plt.title("Histogram of Normally Distributed Data")
plt.xlabel("Value")
plt.ylabel("Probability Density")
plt.legend()
plt.grid(True)
plt.show()
```

**Outcome:**
The generated histogram provided a clear visual representation of a normal distribution. I also highlighted the mean and standard deviation on the graph, which helped emphasize the key characteristics of the dataset. This task solidified my understanding of generating and analyzing random numbers in Python using statistical methods.

---

#### Task 3: Generating a Random Point in a Square

**Description:**
In this final task, I generated a random point uniformly distributed inside a square. The exercise aimed to visualize how random points can be placed within a bounded area.

**Code Example:**
```python
# Define a function to generate a random point inside a square
a = np.random.uniform(5)
def generate_point(a):
    x1 = np.random.uniform(0, a)
    y1 = np.random.uniform(0, a)
    return x1, y1

# Visualize the point inside the square
x1, y1 = generate_point(a)
plt.figure(figsize=(10, 6))
plt.scatter(x1, y1, s=50, color="red", alpha=0.7, edgecolors="black", linewidths=1)
plt.xlim(0, a)
plt.ylim(0, a)
plt.xlabel("X-axis")
plt.ylabel("Y-axis")
plt.title("Random Point in a Square")
plt.grid(True)
plt.show()
```

**Outcome:**
This simple but effective task showed how random points can be uniformly distributed in a 2D space. It allowed me to explore concepts of randomness in spatial dimensions, which could be applied to more complex simulations involving spatial modeling.

---

### Group Project 5: Epidemiology Simulation in Scientific Programming

**Overview:**
This group project focused on modeling an epidemic's dynamics using mathematical and computational approaches. We implemented the SIR (Susceptible, Infected, Recovered) model to simulate an isolated population's reaction to an infectious disease.

**Team Members:**
- Anastasiya Suponina
- Mikhail Lobov
- Vsevolod Rajendran Nirdoshi

#### Key Concepts:

- **SIR Model:** A classic epidemiological model that divides the population into three categories: susceptible (S), infected (I), and recovered (R). The model's dynamics were captured through differential equations describing the rates of change for each group.
  
- **Model Equations:**
  We implemented the core equations of the SIR model, which define how the number of infected and susceptible individuals changes over time:
  \[
  \frac{dS}{dt} = -\beta \cdot S \cdot I
  \]
  \[
  \frac{dI}{dt} = \beta \cdot S \cdot I - \gamma \cdot I
  \]
  \[
  \frac{dR}{dt} = \gamma \cdot I
  \]
  Here, \(\beta\) represents the infection rate, and \(\gamma\) is the recovery rate. These equations were integrated over time to simulate the spread of the infection.

#### Implementation:

We used Python libraries like NumPy and SciPy to implement the model, and Matplotlib for visualizing the results. 

**Key Steps:**
1. Defined initial conditions for the number of susceptible, infected, and recovered individuals in the population.
2. Solved the system of differential equations using numerical methods.
3. Visualized the results to show how the number of infected individuals evolves over time.

**Conclusion:**
This project helped us understand the critical importance of mathematical models in epidemiology. The SIR model, though simple, provided powerful insights into how an infectious disease spreads and how measures like isolation can impact the dynamics of an epidemic. 

---

### SQL Database Project

**Description:**
In parallel, I also worked on structuring a database using SQL. This project involved designing and implementing a database that could efficiently store and manage data related to various products.

**SQL Script:**
```sql
CREATE TABLE Products (
    ProductID INT PRIMARY KEY,
    ProductName VARCHAR(255),
    Price DECIMAL(10, 2),
    Stock INT
);

INSERT INTO Products (ProductID, ProductName, Price, Stock) VALUES
(1, 'Laptop', 1200.00, 10),
(2, 'Mouse', 20.00, 150),
(3, 'Keyboard', 30.00, 80);

-- Query to retrieve all products
SELECT * FROM Products;
```

**Outcome:**
The SQL script successfully created a "Products" table and inserted sample data. This project helped reinforce my skills in SQL database management and the ability to organize data effectively for querying and updates.

---

This week was filled with various coding challenges, each focusing on different domains of programming, from Python-based simulations to database management with SQL. Each project provided valuable insights and practical skills, which I plan to build upon in future work.