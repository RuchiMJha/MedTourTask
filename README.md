# MedTourTask: Bayesian Analysis of Handedness and Age at Death

This project explores the relationship between handedness and age at death using real-world data and Bayesian probability. Inspired by a study that claimed left-handed individuals die younger, we investigate whether this age gap is a statistical artifact caused by changing rates of left-handedness over time.

## Overview

We use survey data on handedness by age and national death distribution statistics to build a probabilistic model. By applying Bayes’ theorem, we estimate the likelihood of dying at a certain age given handedness, and compare left- and right-handed populations.

## Steps in the Analysis

### a. Step 1: Importing Data and Visualizing Handedness by Age
- Load essential Python libraries (`pandas`, `matplotlib.pyplot`)
- Read the handedness dataset into a DataFrame
- Generate a scatter plot showing how left-handedness varies with age for both males and females

### b. Step 2: Enhancing the Dataset with Birth Year and Average Handedness
- Add a column estimating each individual's birth year based on age
- Compute average left-handedness across genders
- Plot average left-handedness vs. birth year to observe trends

### c. Step 3: Estimating P(Left-Handed | Age at Death)
- Use `numpy` for numerical operations
- Estimate left-handedness rates for early and late 1900s births
- Assign rates to age groups to estimate P(LH | A)

### d. Step 4: Loading and Plotting Death Distribution Data
- Import death statistics from a public dataset (1999 US data)
- Clean the data by removing missing values
- Plot the number of deaths by age

### e. Step 5: Computing Overall Left-Handedness Probability
- Define a function to calculate P(LH) for the deceased population
- Weight age-specific left-handedness by death counts
- Normalize to get the overall probability

### f. Step 6: Determining Conditional Probability of Death for Left-Handers
- Build a function to calculate P(A | LH) using Bayes’ theorem
- Combine P(LH | A), P(A), and P(LH)

### g. Step 7: Determining Conditional Probability of Death for Right-Handers
- Create a similar function for right-handed individuals
- Use complementary probabilities to estimate P(A | RH)

### h. Step 8: Visualizing Death Probabilities by Handedness
- Calculate P(A | LH) and P(A | RH) for ages 6 to 120
- Plot both distributions to compare visually

### i. Step 9: Calculating Average Age at Death for Each Group
- Multiply each age by its corresponding probability
- Sum to find the mean age at death for left- and right-handers
- Display the averages and highlight the difference

### j. Step 10: Updating the Analysis for a New Study Year
- Change the study year to 2025 in your functions
- Recalculate all probabilities and averages
- Observe how the age gap changes with stabilized handedness rates

##  Files
- `handedness_data.csv`: Survey data on handedness by age and gender
- `death_distribution_data.csv`: US death statistics by age (1999)
- `MedTourTask.ipynb`: Main analysis notebook

##  Key Insight
The observed age gap between left- and right-handers is largely due to historical shifts in handedness reporting. Left-handed individuals are not inherently more likely to die younger — the data reflects generational bias, not biological fate.

---

Let me know if you'd like a short project summary or tagline for the repo description too!
