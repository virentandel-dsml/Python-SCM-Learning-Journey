# Supplier Performance & Risk Assessment System

## Business Problem

Procurement teams often evaluate suppliers using several performance measures rather than a single KPI.

This project demonstrates a simple rule-based approach to assess suppliers across three areas:

1. Delivery performance
2. Quality performance
3. Procurement price performance

The objective is to move from individual KPI calculations to an overall supplier assessment and a recommended procurement action.

## Objective

For each supplier, the program:

- Calculates delivery performance
- Calculates defect rate
- Calculates procurement price variance
- Converts each KPI into a performance score
- Calculates an overall supplier score
- Identifies the weakest KPI as the risk driver
- Classifies the supplier
- Recommends a procurement action

## Synthetic Data

The project uses fictional supplier names:

- Apex Components
- Vertex Industrial
- Nova Engineering
- Prime Tech Manufacturing

No real supplier or company data is used.

## KPI Logic

### 1. Delivery Performance

Delivery delay is calculated as:

```text
Actual Delivery Days − Promised Delivery Days
```

Classification:

| Condition | Score |
|---|---:|
| On time | 3 |
| 1–2 days late | 2 |
| More than 2 days late | 1 |

### 2. Quality Performance

Defect rate is calculated as:

```text
Defective Quantity / Received Quantity × 100
```

Classification:

| Defect Rate | Score |
|---|---:|
| ≤ 2% | 3 |
| > 2% and ≤ 5% | 2 |
| > 5% | 1 |

### 3. Procurement Price Performance

Price variance is calculated as:

```text
Actual Price − Standard Price
```

Classification:

| Price Variance | Score |
|---|---:|
| ≤ 0 | 3 |
| > 0 and ≤ 10 | 2 |
| > 10 | 1 |

## Overall Supplier Score

The three KPI scores are combined:

```text
Overall Score = Delivery Score + Quality Score + Price Score
```

Assessment:

| Overall Score | Assessment |
|---|---|
| 8–9 | Strong Supplier |
| 6–7 | Moderate Risk |
| 3–5 | High Risk |

## Risk Driver

The lowest KPI score is used to identify the supplier's primary risk driver:

- Delivery
- Quality
- Price

This provides a simple explanation of **why** a supplier requires attention.

## Recommended Procurement Action

The assessment is translated into an action:

| Situation | Recommended Action |
|---|---|
| Strong Supplier | Continue / Preferred Supplier |
| Moderate Risk | Monitor the identified performance area |
| High Risk | Supplier Improvement Required, focused on the identified risk area |

## Python Concepts Used

The project was deliberately built using concepts covered during the Week 1 and Week 2 learning period:

- Lists
- List indexing
- `for` loops
- `enumerate()`
- `zip()`
- `if / elif / else`
- Arithmetic calculations
- `round()`
- f-strings

No external data-science libraries are required for this exercise.

## Business Flow

```text
Supplier Data
      ↓
Delivery KPI
Quality KPI
Price KPI
      ↓
Individual KPI Scores
      ↓
Overall Supplier Score
      ↓
Risk Driver
      ↓
Supplier Assessment
      ↓
Recommended Procurement Action
```

## Key Learning

The main learning from this project was the transition from calculating individual SCM metrics to combining multiple KPIs into a rule-based business decision.

The project is intentionally a foundation rather than a machine-learning model. More advanced analytics, statistical methods, and ML techniques can be introduced as the Python and Supply Chain Analytics learning journey progresses.

## Disclaimer

This is a learning/portfolio project. All supplier names and data are synthetic and do not represent actual companies or supplier performance.
