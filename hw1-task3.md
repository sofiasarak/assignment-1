# Homework 1 Task 3

---

Answer the following questions based on exercises from *An Introduction to Statistical Learning with Applications in Python*.

## Chapter 2.4 Exercises

---

### Exercise 1 (ISLP exercise 2)

Explain whether each scenario is a **classification or regression** problem, and indicate whether we are most interested in **inference or prediction**. Finally, provide **n** (size of observation dataset) and **p** (number of predictors).

**(a)**  We collect data on 200 protected marine reserves worldwide. For each reserve we record species richness, reserve size, years since establishment, enforcement budget, and proximity to human settlements. We are interested in understanding which factors affect species richness.

> **Your Answer:** regression; inference; n = 200; p = 4

---

**(b)** A conservation agency wants to know whether a proposed habitat corridor will successfully support wildlife movement or fail to do so. They collect data on 30 previously established corridors. For each corridor they have recorded whether wildlife movement was successful or unsuccessful, corridor width, length, surrounding land use type, and eight other variables.

> **Your Answer:** classification; prediction; n = 30; p = 11

---

**(c)** We are interested in predicting weekly average ground-level ozone concentration in a coastal city. We collect weekly data for all of 2019. For each week we record average ozone concentration, sea surface temperature, wind speed, solar radiation, and atmospheric

> **Your Answer:** regression; prediction; n = 52; p = 4

---

### Exercise 2 (ISLP exercise 5)

What are the advantages and disadvantages of a very flexible (versus a a less flexible) approach for regression? Under what circumstances might a more flexible approach be preferred to a less flexible approach? When might a less flexible approach be preferred?

> **Your Answer:** A very flexibile approach for regression allows us to fit the training data very well (low training MSE), but the model may perform poorly on test data (high test MSE). A flexible model could lead to over-fitting, where the model finds/learns patterns from the test data that happen by chance, and are not indicative of the true population. 

More flexible: low bias, high variance
Less flexible: high bias, low variance

---

### Exercise 3 (ISLP exercise 6)

Describe the differences between a **parametric** and a **non-parametric** statistical learning approach. What are the **advantages** of a parametric approach to regression or classification (as opposed to a non-parametric approach)? What are its **disadvantages**?

> **Your Answer:** In a parametric statistical learning approach, there is an assumption made about the form of the function. For example, a Simple Linear Regression estimates a linear relationship. Training data is then used to fit this model, calculating the parameters that fit the predefined shape. A parametric approach is advantageous when working with small training data sets, or to make inference easier. Tt can work poorly when the assumed functional form is inaccurate, making parameters and predicitions inaccurate as well. A non-parametric approach does not define its functional form, but creates a model that fits as closely as possible to the data, without being "too rough". This approach may require a lot of data, be susceptible to overfitting, and may be less interpretable, but it could produce more accurate results/be better at prediction.