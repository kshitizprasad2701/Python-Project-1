# Capstone Project: Project Head & Performance Analysis using Python

## Overview

This capstone project focuses on data handling, transformation, and analysis using Python and its data science libraries like Pandas and NumPy. The goal is to simulate real-world tasks such as data cleaning, feature engineering, merging datasets, and applying business rules to update or derive new metrics.

---

## Dataset Description

The project uses data split into three main datasets:

### 1. Employee Data
Details of project heads handling various projects.
| Attribute | Description |
|----------|-------------|
| ID       | Unique identifier for the project head |
| Name     | Full name of the project head |
| Gender   | Gender of the project head (M/F) |
| City     | Location of the project |
| Age      | Active years of the project |

### 2. Seniority Level
Represents the position of the project head.
- Designation Level Scale:
  - 1 = Highest
  - 2, 3 = Mid-level
  - 4 = Entry-level
  - >4 = Not eligible to lead a project

### 3. Project Data
Details of the projects handled by employees.
| Attribute | Description |
|----------|-------------|
| ID       | Refers to the project head |
| Project  | Project Name |
| Cost     | Project cost (some values missing) |
| Status   | Project status (Finished/Ongoing/Failed) |

---

## Tasks

### Task 1
- Create and save three DataFrames: `Employee.csv`, `Seniority.csv`, `Project.csv`.

### Task 2
- Replace missing values in the `Project` cost using **running average** (with a for loop).

### Task 3
- Split the `Name` column into `First Name` and `Last Name`.

### Task 4
- Merge all three DataFrames into one called `Final`.

### Task 5
- Add a `Bonus` column:
  - 5% bonus on `Project Cost` for employees with `Finished` projects.

### Task 6
- **Demotion**:
  - Reduce designation level by 1 for employees with `Failed` projects.
  - Remove employees with designation level > 4.

### Task 7
- Prefix `Mr.` or `Mrs.` to `First Name` based on `Gender`.
- Drop the `Gender` column.

### Task 8
- **Promotion**:
  - Promote designation by 1 if employee age > 29.

### Task 9
- Create a new DataFrame `TotalProjCost` with:
  - `ID`, `First Name`, `Total Cost` of projects.

### Task 10
- Print employee details where the city name contains the letter **"o"**.

---

## Tools & Libraries Used

- Python 3.x
- Pandas
- NumPy
- Jupyter Notebook (`.ipynb`)

---
