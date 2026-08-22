# Transportation Performance Analysis using NumPy

## Project Overview

This project applies **NumPy** to a practical Supply Chain Management (SCM) performance-analysis problem focused on **transportation service and cost performance**.

The analysis evaluates **OTIF (On-Time In-Full)** and **Freight Cost** across transportation routes and weeks, then combines these metrics to identify areas requiring management attention.

## Business Objectives

The analysis is designed to answer:

- Which transportation routes are underperforming on OTIF?
- Which weeks show weaker transportation service performance?
- Which routes have the highest average freight cost?
- Which weeks have the highest average freight cost?
- Which routes combine **below-benchmark OTIF** with **above-average freight cost**?

## Dataset Structure

The project uses NumPy arrays representing:

- **4 transportation routes**
- **5 weeks**
- Route-level and week-level OTIF performance
- Freight cost data in **₹'000**

Rows represent routes and columns represent weeks.

## Key Analysis Performed

### 1. OTIF Performance Analysis

- Calculated overall OTIF benchmark
- Calculated route-wise average OTIF
- Measured route variance against the benchmark
- Identified underperforming routes
- Identified the worst-performing route
- Calculated weekly average OTIF
- Identified the weakest week
- Applied a threshold to flag significant underperformance

### 2. Freight Cost Analysis

- Calculated total freight cost
- Calculated route-wise average freight cost
- Identified the highest-cost route
- Calculated weekly average freight cost
- Identified the highest-cost week

### 3. Integrated Performance Analysis

The project combines service and cost metrics to identify routes that have:

- **Below-benchmark OTIF**, and
- **Above-average freight cost**

This creates a practical prioritization approach for transportation performance improvement.

## Key Business Finding

**Mumbai - Bengaluru** emerged as the priority route because it combines **below-benchmark OTIF performance** with **above-average freight cost**.

This indicates an opportunity to investigate the route for potential service and transportation-cost improvement.

## NumPy Concepts Applied

The project demonstrates practical use of:

- NumPy arrays
- Array dimensions and `shape`
- `ndim`
- `axis`
- `np.mean()`
- `np.sum()`
- `np.argmax()`
- `np.argmin()`
- Array indexing
- Boolean masking
- Combining Boolean conditions
- Basic array operations

## Business Value

The project demonstrates how Python and NumPy can be used not just for programming practice, but to transform SCM performance data into **KPI-driven business insights**.

The analytical flow is:

**Data → KPI Calculation → Performance Comparison → Business Finding**

## Tools & Technologies

- Python
- NumPy
- Jupyter Notebook

## Project File

`Transportation_Performance_Analysis(2).ipynb`

## Learning Context

This project was developed as part of **Week 3 of my Python learning journey**, with a focus on applying NumPy concepts to real-world Supply Chain Analytics scenarios.
