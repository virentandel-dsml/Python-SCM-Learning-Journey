# Week 2 — Python for Supply Chain Analytics

## Overview

Week 2 focused on moving from basic Python syntax toward applying Python control flow and business rules to practical Supply Chain Management scenarios.

The goal was not to learn Python in isolation, but to use Python as a tool for solving SCM problems.

## Learning Progression

- **Day 1:** Understand the concepts — learning from instructional material, without practice
- **Day 2:** Practice simple SCM problems
- **Day 3:** Practice slightly more complex SCM problems
- **Day 4:** Build a larger SCM-focused practice project
- **Day 5:** Consolidate the learning and prepare the work for GitHub and LinkedIn

## Python Concepts Practiced

- Variables
- Numbers and arithmetic
- Strings
- Lists
- List indexing
- `if / elif / else`
- `for` loops
- `range()`
- `enumerate()`
- Nested loops
- `zip()`
- `while` loops
- f-strings
- `round()`

## SCM Areas Practiced

The exercises applied Python to multiple SCM scenarios, including:

- Inventory replenishment
- Order fulfillment and backorders
- Cycle count / inventory variance
- Supplier lead time
- Supplier delivery performance
- Procurement price variance
- Production capacity
- Transportation cost
- Warehouse utilization
- Machine availability
- Demand vs. forecast variance
- Order picking accuracy
- Production scrap rate
- Supplier quality / defect rate

## Week 2 Flagship Project

### Supplier Performance & Risk Assessment System

The Day 4 project combined multiple supplier performance dimensions into a rule-based assessment:

**Delivery Performance → Quality Performance → Price Performance → KPI Scores → Overall Supplier Score → Risk Driver → Recommended Procurement Action**

The project demonstrates how Python conditional logic can be used to translate SCM business rules into an operational decision framework.

### Assessment dimensions

- Delivery performance
- Defect / quality performance
- Procurement price variance
- Overall supplier score
- Weakest KPI / risk driver
- Recommended procurement action

## Repository Structure

```text
Week-2-Python-for-Supply-Chain/
│
├── README.md
│
├── Day-2-Practice/
│   └── Week_2_Basics_1.ipynb
│
├── Day-3-Practice/
│   └── Week_2_Basics_2.ipynb
│
└── Day-4-Flagship-Project/
    ├── Supplier_Performance_Risk_Assessment.ipynb
    └── README.md
```

## Key Learning

The main progression in Week 2 was from solving individual SCM calculations to combining multiple KPIs and business rules into a single supplier assessment.

This is an early step toward using Python for Supply Chain Analytics, with more advanced data analysis and machine learning to be explored in later stages.

## Note

This repository represents a learning project. The supplier names and data are synthetic and are used for practice purposes only.
