# 📊 Supervised Learning Methods in R: A Practical Portfolio 📈

<p align="center">
    <!-- Project Links -->
    <a href="https://github.com/Silvestre17/SupervisedLearningR_Portfolio"><img src="https://img.shields.io/badge/Project_Repo-100000?style=for-the-badge&logo=github&logoColor=white" alt="GitHub Repo"></a>
</p>

## 📝 Description

This repository is a collection of projects and assignments developed for the **Supervised Learning Methods** course. It showcases the practical application of various regression and classification techniques to solve real-world problems. All analysis, modeling, and reporting were conducted using the **R programming language** and its rich ecosystem of statistical packages.

## ✨ Learning Objectives

This portfolio demonstrates the development of core competencies in supervised machine learning, directly addressing the course's learning goals:
*   Understanding the scope and procedures of various **supervised learning methods**.
*   Proficiently using the **R software** and RStudio for complex data analysis.
*   Critically **evaluating and interpreting** the results of predictive models.

## 🎓 Project Context

This work was completed for the **Métodos de Aprendizagem Supervisionada** (*Supervised Learning Methods*) course as part of the **[Licenciatura em Ciência de Dados](https://www.iscte-iul.pt/degree/code/0322/bachelor-degree-in-data-science)** (*Bachelor Degree in Data Science*) at **ISCTE-IUL**, during the 2022/2023 academic year (2nd Semester of 2nd Year).

## 🛠️ Technologies Used

The entire workflow, from data exploration to modeling and reporting, was executed using R and its powerful libraries.

<p align="center">
    <a href="https://www.r-project.org/">
        <img src="https://img.shields.io/badge/R-276DC3?style=for-the-badge&logo=r&logoColor=white" alt="R" />
    </a>
    <a href="https://www.rstudio.com/">
        <img src="https://img.shields.io/badge/RStudio-75AADB?style=for-the-badge&logo=rstudio&logoColor=white" alt="RStudio" />
    </a>
    <a href="https://rmarkdown.rstudio.com/">
        <img src="https://img.shields.io/badge/R_Markdown-5178B8?style=for-the-badge&logo=r&logoColor=white" alt="R Markdown" />
    </a>
</p>

#### Key Libraries
*   **Modeling & Machine Learning:** `nnet` (for Multinomial Logistic Regression), `tree` (for Classification Trees), `caret`, `e1071`, `FNN` (for K-Nearest Neighbors).
*   **Data Analysis & Utilities:** `HSAUR2` (for datasets like CHFLS), `MASS`, `psych`, `lsr`, `car`, `Metrics`.
*   **Data Visualization:** `ggplot2` for creating insightful plots.

---

## 📚 Project Breakdown

This repository contains two main projects, each tackling a different supervised learning problem.

### 1️⃣ Project: Predicting Happiness (CHFLS Dataset)

This project focused on **multinomial classification** to predict the self-reported happiness level (`R_happy`) of individuals from the China Health and Family Life Survey (CHFLS).

<p align="center">
    <img src="https://img.shields.io/badge/Task-Classification-blue" alt="Classification Task"/>
</p>

#### Key Concepts & Methods Implemented:
*   **Feature Selection:** Used **Cramer's V** to measure the association between the categorical target variable (`R_happy`) and other qualitative predictors to select the most relevant feature (`R_health`).
*   **Multinomial Logistic Regression:** Implemented a regression model using the `nnet` package to predict outcomes across multiple, unordered happiness categories.
*   **Classification Tree:** Built a decision tree using the `tree` package and applied **cost-complexity pruning** (`prune.tree`) to find the optimal tree size and prevent overfitting.
*   **Model Evaluation:** Assessed model performance by generating **Confusion Matrices** and calculating key metrics like overall **accuracy**.

### 2️⃣ Project: Predicting Youth Consumer Behavior

This project involved both **regression** and **classification** tasks to analyze the purchasing habits of young consumers from the "Consumo.Jovens.csv" dataset.

<p align="center">
    <img src="https://img.shields.io/badge/Task-Regression%20%26%20Classification-purple" alt="Regression and Classification Tasks"/>
</p>

#### Key Concepts & Methods Implemented:
*   **K-Nearest Neighbors (KNN) Regression:**
    *   Implemented KNN to predict a continuous variable (`q19_8`).
    *   Performed **hyperparameter tuning** by iterating through different values of `K` and selecting the optimal `K` that minimized the **Sum of Squared Errors (SSE)**.
*   **Classification Tree for Brand Purchase Prediction:**
    *   Constructed a decision tree to predict a binary outcome: whether a consumer buys brand-name products (`q10`).
    *   The model was built using predictors related to shopping habits and product preferences (`q12b_a`, `q13a`, etc.).
    *   Applied **pruning** to simplify the tree and improve its generalizability.
*   **Hold-Out Validation:** The dataset was split into **training (60%)** and **testing (40%)** sets to ensure a robust evaluation of the models' performance on unseen data.

## 🚀 How to Run the Solutions

Each project is contained within its own set of files. To view or reproduce the results:

1.  **Prerequisites:**
    *   Install [R](https://www.r-project.org/).
    *   Install [RStudio Desktop](https://www.rstudio.com/products/rstudio/download/).
2.  **Open the Project:**
    *   Navigate to the folder of the project you wish to review.
    *   Open the `.Rmd` (R Markdown) file in RStudio.
3.  **Install Required Packages:**
    *   At the beginning of each script, there is a list of required libraries. Install any missing packages by running `install.packages("package_name")` in the RStudio console.
4.  **Generate the Report:**
    *   Click the **"Knit"** button in the RStudio toolbar. This will execute all the R code within the document and compile a final, formatted report in `.html` or `.pdf` format.

## 🇵🇹 Note

These assignments were developed and written in Portuguese from Portugal 🇵🇹.