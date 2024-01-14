# Project Name
> Analysis of parameters indicating a loan being sanctioned could be defaulted


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.
When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. 
- What is the background of your project?
Borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 
If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.
- What is the business probem that your project is trying to solve?
The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.
- What is the dataset that is being used?
The data given in a csv contains information about past loan applicants and whether they ‘defaulted’ or not. 

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- Default rate continuously increases from Loan grade A to G and is exceptionally high beyond E which has 26%. F and G are more than 32 %. Loans in this category need special scrutiny.
- Purpose marked Small_business has a very high default rate of 26%. This shows that small business run a risk of not being able to pay as they might not survive tough business situations.
- Loans with Term of 60 months has a significantly higher default rate of 25% than that of 36 months which is only at 10%. Company may need to put more stringent checks on terms with 60 months.
-  Non-verified loans have much lower defaults of 12% while Verified ones have a default of 16%. This might be a sign that the verification process has gaps and we are better off with third party verification. Non verified loans are possibly known to be safe bets and hence have an expected lower defaults. These are probably reliable and known customers.
 - funded_amnt_inv more than 15000 has a significantly high default rate of 18%.
The default rate decreases with the decreasing funded amount by investors but increases at the lowest bin i.e. below 4448.
- annual_inc has a negative correlation with the default rate. In the lowest income group [below 37000] the default rate is 17%. There is an opportunity to reduce the default rate for customers with income below 37000.
- dti has a direct correlation with the default rate. The default rate increases to nearly 17% for dti above 19. This is expected as customers with high debt payments to their monthly pay are possibly under financial strain. This needs to be checked during approval.
- Defaults increase with increasing interest rate but in the highest bin of 15% and above the defaults are exceptionally high at 26%. Infact, this is one of the biggest indicator of a high default. Ideally, Lending Club should reconsider if they should even allow rates beyond 15%. Or make it clear to investors that such rates can cause a 1/4 chance of a default. So investors are aware of the risk associated with such high returns
- from Bivariate analysis of employment years vs loan issue year heatmap: we notice high default rates on loan issued in the year 2007 but especially so for employment years of 4, 7, 8, and 10+. Interestingly employees with 2 yrs of experience did quite well with only 8% defaulting in an otherwise bad year for issuing loans.
- From BiVariate analysis of home ownership vs purpose heatmap: we see 100% default with the combination of Moving as Purpose and Other as home Ownership and also a default of 50% with
 a combination of Car as Purpose and Other as Home ownerhsip. Small Business as purpose was a high rate of default in the univariate analysis. But now we can see that in this category even customers who own a home also default to a high rate of 33%. The purpose code of Renewal Energy with customers who are on Rent has a high default rate of 25%.
<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python 3.11.1
- Pandas 2.1.4
- Numpy 1.26.3 
- Seaborn 0.13.1

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by...
- References if any...
- This project was based on [this tutorial](https://www.example.com).


## Contact
Created by [@anilabh and @samik0701]


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->