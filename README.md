# MedTourTask
a. Step 1: Importing Data and Visualizing Handedness by Age
Load essential Python libraries like pandas and matplotlib.pyplot
Read the handedness dataset into a DataFrame
Generate a scatter plot to show how left-handedness varies with age for both males and females
b. Step 2: Enhancing the Dataset with Birth Year and Average Handedness
Add a new column to estimate each individual's birth year based on their age
Compute the average left-handedness across genders and store it in a new column
Plot this average against birth year to observe trends over time
c. Step 3: Estimating P(Left-Handed | Age at Death)
Use numpy for numerical operations
Determine average left-handedness rates for people born in the early and late 1900s
Assign appropriate rates to different age groups to estimate the likelihood of being left-handed at death
d. Step 4: Loading and Plotting Death Distribution Data
Import death statistics from a given URL into a DataFrame
Clean the data by removing missing values
Create a plot showing how many people died at each age
e. Step 5: Computing Overall Left-Handedness Probability
Define a function to calculate the general probability of being left-handed in the deceased population for a specific year
Multiply age-specific death counts by their corresponding left-handedness probabilities
Sum and normalize the results to get the overall likelihood
f. Step 6: Determining Conditional Probability of Death for Left-Handers
Build a function to calculate the chance of dying at a certain age, given that the person was left-handed
Use death data and previously computed probabilities to apply Bayes’ theorem
g. Step 7: Determining Conditional Probability of Death for Right-Handers
Create a similar function for right-handed individuals
Use complementary probabilities to estimate P(Age at Death | Right-Handed)
h. Step 8: Visualizing Death Probabilities by Handedness
Calculate conditional probabilities for a range of ages
Plot both left- and right-handed death distributions to compare visually
i. Step 9: Calculating Average Age at Death for Each Group
Multiply each age by its corresponding probability for both groups
Sum the results to find the mean age at death for left- and right-handers
Display the averages and highlight the difference
j. Step 10: Updating the Analysis for a New Study Year
Change the study year to 2018 in your functions
Recalculate all relevant probabilities and averages based on this updated context
