# Bayesian Poisson Regression on Seatbelts Data

This project applies **Bayesian Poisson Regression** using **JAGS** to the classic R dataset `Seatbelts`. The target variable is `VanKilled`, while the predictors include other features in the dataset.

## 📊 Dataset

The `Seatbelts` dataset is a built-in R dataset that records monthly UK road accident casualties from 1969–1984. In this notebook:

* **Target**: `VanKilled` (number of van drivers killed or seriously injured)
* **Predictors**: Other covariates from the dataset (e.g., PetrolPrice, kms, etc.).

## 🧩 Methodology

1. **Model**:

   * Response: Poisson distributed,
   * Link: Log link,
   * Priors: Weakly informative Gaussian priors for coefficients.

2. **Diagnostics**:

   * Geweke diagnostic,
   * Gelman-Rubin R-hat statistic,
   * Effective sample size.

3. **Model Fit Criteria**:

   * DIC (Deviance Information Criterion),
   * WAIC (Watanabe-Akaike Information Criterion).

4. **Posterior Predictive Checks**:

   * Generated posterior predictive distributions,
   * Compared simulated outcomes to observed counts.

## 🛠️ Tools Used

* **R**
* **rjags** (for Bayesian inference)
* **coda** (for MCMC diagnostics)

## 📈 Results

* Model coefficients were estimated via Bayesian inference,
* Convergence verified with diagnostics,
* DIC and WAIC computed for model assessment,
* Posterior predictive checks showed reasonable model fit.

## 🚀 How to Run

1. Clone this repository.
2. Open the `.Rmd` or `.R` script in RStudio.
3. Ensure `rjags` and `coda` packages are installed.
4. Knit the notebook to HTML or run chunks interactively.

---

📌 This project is part of my Bayesian statistics practice, focusing on regression models, MCMC diagnostics, and predictive checks.
