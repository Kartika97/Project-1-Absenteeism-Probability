# Absenteeism Project : Project Overview

To see the probability when the employee will leave their desk at work through 8 variables;
* Reasons
* Month value
* Transportation Expense
* Age
* BMI
* Education 
* Children
* Pet

# Code and Resources Used
Phyton version  : Python 3.7
Packages        : NumPy, Pandas, Pickle
Raw data        : Udemy - 365Carrers

# Data Cleaning
From the raw data I received, I have to clean it up so it was usable for our model. I made the following changes and created the following variables:

* Splitting a variable into mutiple dummy variable from 'Reason for Absence' coloumn into Reason_1, Reason_2, Reason_3, and Reason_4. (There were 28 reasons from the raw data, I grouped it so that it easier to understand, where Reason_1 1:14, Reason_2 15:17, Reason_3 18:21, Reason_4 22:28)
* Retrieving month value from 'Date' coloumn
* Make a dummy variable from 'Education' coloumns (1:0, 2:1, 3:1, 4:1). 1 = HS graduate 2-4 = post-graduate, masters, Phd
* Drop several coloumns as we don't need them (ID, Reason for Absence, Date, Absenteeism Time in Hours)

# EDA 
[Tableau Public link](https://public.tableau.com/app/profile/tara5851/viz/Absenteeism_Probability_16436227906760/Story1) ;))

![alt text](https://github.com/Kartika97/Project-1-Absenteeism-Probability/blob/main/Age%20vs%20Probability.png "Age vs Probability")

![alt text](https://github.com/Kartika97/Project-1-Absenteeism-Probability/blob/main/Transportation%20Expense%20with%20Number%20of%20Children%20vs%20Probability.png " Reasons of Absence vs Probability")

* Reason_1 = reason 1 to 14, Represent very serious diseases.
  *The reason_1 we have here represent very serious diseases. That's why the numbers tell us that the expected probability of an individual to be excessively absent because of a reason from this class is higher than 50 percent.*
* Reason_2 = reason 15 to 17, Represent Pregnancy/ Maternal matters.
* Reason_3 = reason 18 to 21 Represent Poisoning matters.
* Reason_4 = reason 22 to 28 Represent light reasons for absence, a dental appointment, physiotherapy, a medical consultation and others. 
  *It is quite probable that none of these could be serious enough to require that a person is absent from their workplace for an entire day. That's why the numbers show that people who have to be absent for such a reason are not expected to be excessively absent.*

![alt text](https://raw.githubusercontent.com/Kartika97/Project1_Absenteeism/e9807b3a70935d29c60967b20e7f324d8121c52d/Transportation%20Expense%20with%20Number%20of%20Children%20vs%20Probability.png " Transportation Expense with Number of Children vs Probability")
