# VoltRelay Network Analysis

## Overview

VoltRelay is an electric mobility battery-swapping network. This project analyzes the network's operational and commercial performance using observational data to identify patterns associated with service failures, rider retention, equipment reliability, and partner economics.

The analysis covers network performance, service quality, station and geographic patterns, battery and equipment performance, pricing and partner economics, and rider retention.

## Objectives

The analysis addresses six key business questions:

1. How did network performance change over time?
2. What factors are associated with service failures and customer experience?
3. How do station, geographic, and infrastructure characteristics vary with performance?
4. What battery and equipment characteristics are associated with failures?
5. How do pricing structures and fleet partner contracts affect revenue performance?
6. What factors are associated with rider retention?

## Dataset

The project uses eight datasets covering:

* Swap events
* Station hourly status
* Riders
* Batteries
* Support tickets
* Stations
* City-level daily context
* Fleet partners

The analysis uses observational data, so the findings describe associations and patterns rather than establishing causality.

## Analysis Areas

### 1. Network Performance

Examines:

* Swap volume
* Revenue
* Failure rates
* Revenue per completed swap
* Performance trends over time

### 2. Service Failures & Customer Experience

Examines:

* Failed swaps
* Queue waiting time
* Abandoned swaps
* Station and city-level differences
* Charger generation
* Customer experience patterns

### 3. Station & Geographic Patterns

Examines how:

* Station characteristics
* Charger generations
* Geographic location
* Commissioning waves
* Operational conditions

relate to network performance.

### 4. Battery & Equipment Performance

Examines:

* Battery state of health
* Battery suppliers
* Manufacturing lots
* Charger generations
* Failure patterns across equipment cohorts

### 5. Pricing & Partner Economics

Examines:

* Tariff structures
* Partner discounts
* Revenue per swap
* Fleet partner economics
* Contract amendments

A notable finding was the ZipDrop contract amendment, where the contracted discount increased from 12% to 28%. The observed post-amendment revenue per swap decreased from ₹57.48 to ₹48.65. The post-amendment period is short, so this is treated as an observed association rather than a causal conclusion.

### 6. Rider Retention

Examines:

* 1-day, 7-day and 30-day return behavior
* First-swap waiting time
* Prior first-swap failure
* Failure type
* Rider engagement
* City and fleet partner differences

First-swap waiting time and prior failure did not show strong differences in short-term return behavior, while rider engagement showed greater observed variation.

## Key Findings

* Network swap volume and revenue increased substantially over the observed period.
* Failure rates temporarily increased during April–June despite continued network growth.
* Later battery manufacturing lots showed higher observed failure rates than earlier lots.
* Gen 1 chargers showed higher observed failure rates than newer charger generations.
* Battery state of health alone did not clearly distinguish failed and completed swaps.
* PARTNER transactions represented 64.59% of observed revenue.
* Partner discounts and contract structures produced substantial variation in realized revenue per swap.
* Rider first-swap waiting time showed little difference between riders who returned and those who did not.
* Rider engagement showed stronger variation in repeat behavior than the tested first-swap friction variables.

## Recommendations

Based on the observed evidence, VoltRelay should focus on:

1. **Improving equipment reliability**
   Investigate affected battery manufacturing lots and older charger generations.

2. **Protecting partner unit economics**
   Monitor partner discounts, contract terms, revenue per swap, and contribution margin.

3. **Reviewing major contract amendments**
   Evaluate large changes in partner discounts against their impact on volume and economics.

4. **Scaling without sacrificing reliability**
   Track service-quality metrics alongside network expansion and transaction growth.

5. **Monitoring rider engagement**
   Track early engagement and repeat behavior across rider and partner segments.

## Project Structure

```text
VoltRelay-Network-Analysis/
│
├── VoltRelay_Network_Analysis.ipynb
└── README.md
```

## Methodology

The analysis follows an evidence-based exploratory approach:

```text
Data Loading
     ↓
Data Cleaning & Validation
     ↓
KPI Construction
     ↓
Trend Analysis
     ↓
Failure & Equipment Analysis
     ↓
Geographic & Station Analysis
     ↓
Pricing & Partner Analysis
     ↓
Retention Analysis
     ↓
Cross-Factor Synthesis
     ↓
Prioritization
```

## Limitations

* The analysis is observational and does not establish causality.
* Some post-intervention periods are short.
* Observed relationships may be influenced by other operational or customer-level factors.
* Rider engagement is partly constructed from subsequent usage behavior and should therefore not be interpreted as an independent causal driver.
* Additional controlled experiments and longer observation periods would strengthen the findings.

## Project Deliverable

The detailed analysis, calculations, tables, and conclusions are available in the accompanying Jupyter/Google Colab notebook.

**Author:** P S Charitha 
**Project:** VoltRelay_Network_Analysis

````

### Then commit it

At the bottom of GitHub:

**Commit changes**

Use:

```text
Add project README
````

After that your repo will have:

```text
📁 VoltRelay-Network-Analysis
 ├── 📓 VoltRelay_Network_Analysis.ipynb
 └── 📄 README.md
