# Clustering Youth Risk Behavior Data



This repository presents a comprehensive clustering analysis of youth responses from the [Youth Risk Behavior Surveillance System (YRBSS)](https://www.cdc.gov/yrbs/data/index.html). The goal of this project is to identify **latent psychosocial subgroups** among adolescents by clustering participants based on mental health status, environmental stressors, and behavioral risk indicators.


---

## 🎯 Project Objective

To discover **distinct youth profiles** that reflect combinations of risk and resilience factors across multiple domains (e.g., home, social, physical health, substance use). The goal is to inform early intervention strategies by:

- Identifying subgroups with elevated mental health risks
- Detecting overlapping behavioral and emotional vulnerabilities
- Differentiating between high-risk and well-regulated student profiles

---

## 📚 Dataset Description

- **Source**: 2023 National Youth Risk Behavior Surveillance System (YRBSS)
- **Publisher**: U.S. Centers for Disease Control and Prevention (CDC)
- **Sample**: Nationally representative sample of U.S. high school students
- **Topics**: Mental health, substance use, physical activity, violence, suicide, sexual behavior, connectedness, and more
- **Access**: [CDC YRBSS Data Portal](https://www.cdc.gov/yrbs/data/index.html)



## Domain-Wise Clustering

We perform KMeans clustering using **mental health indicators** in conjunction with each of the following contextual domains:
- 🏠 **Home Environment**
- 🧑‍🤝‍🧑 **Social Relationships**
- 🏃‍♀️ **Physical Activity**

This modular approach reveals how different environments relate to patterns of mental distress.

---

## Full-Model Clustering 
We are currently developing a model that clusters across all domains simultaneously, including:
- Mental Health
- Home Environment
- Social Environment
- Physical Activity
- Risk Behaviors (e.g., substance use, violence)

This allows us to assess clustering across the full multidimensional risk space.

---

## ⚙️ Methods Overview

- **Clustering**: We use **KMeans** clustering to group students based on response similarity.
- **Standardization**: All features are standardized using `StandardScaler` to ensure equal contribution.
- **PCA**: Applied for dimensionality reduction and visualization (e.g., scatterplots, density maps).
- **Cluster Evaluation**: We assess cluster structure using:
  - Silhouette Score
  - Calinski–Harabasz Index
  - Davies–Bouldin Index
- **Interpretability**: Cluster labels are manually annotated based on average scores, risk indicators, and visual diagnostics.


---

## Comparison Goals
We aim to:

- Identify whether **similar participant profiles** emerge across domains  
- Assess whether the **full-model clustering** uncovers **additional nuance**  
- Evaluate which approach yields the most **interpretable and actionable clusters**

---

## 📁 Data Access

The dataset used is the **2023 National YRBS**. You can access the raw data from the CDC website:

👉 [CDC YRBSS Data Portal](https://www.cdc.gov/yrbs/data/index.html)

**Note**:  
- The `data_dictionary.md` in the `/data` folder explains selected variables and custom recoding applied in this project.  
- For the official documentation, see: `2023_National_YRBS_Data_Users_Guide.pdf`.

---
## 🙋‍♀️ Authors

- **Emily Han**  
- **Erika Garza-Elorduy**
- **Yawen Dong** 
- **Junyi Hui**

This analysis was conducted as part of an independent research project exploring data-driven strategies for adolescent mental health profiling.

---

## 🙏 Acknowledgments

- Data provided by the **Centers for Disease Control and Prevention (CDC)**  
- We thank the YRBSS team and participating schools for making this dataset publicly available.