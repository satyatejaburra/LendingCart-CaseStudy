# Lending Club Case Study
> consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:
If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company
If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
Introduction
Solving this assignment will give you an idea about how real business problems are solved using EDA. In this case study, apart from applying the techniques you have learnt in EDA, you will also develop a basic understanding of risk analytics in banking and financial services and understand how data is used to minimise the risk of losing money while lending to customers.

  

Business Understanding
You work for a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company

 

The data given below contains information about past loan applicants and whether they ‘defaulted’ or not. The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as denying the loan, reducing the amount of loan, lending (to risky applicants) at a higher interest rate, etc.

 

In this case study, you will use EDA to understand how consumer attributes and loan attributes influence the tendency of default.

Figure 1. Loan Data Set
Figure 1. Loan Data Set
When a person applies for a loan, there are two types of decisions that could be taken by the company:

Loan accepted: If the company approves the loan, there are 3 possible scenarios described below:

Fully paid: Applicant has fully paid the loan (the principal and the interest rate)

Current: Applicant is in the process of paying the instalments, i.e. the tenure of the loan is not yet completed. These candidates are not labelled as 'defaulted'.

Charged-off: Applicant has not paid the instalments in due time for a long period of time, i.e. he/she has defaulted on the loan 

Loan rejected: The company had rejected the loan (because the candidate does not meet their requirements etc.). Since the loan was rejected, there is no transactional history of those applicants with the company and so this data is not available with the company (and thus in this dataset)
 

Business Objectives
This company is the largest online loan marketplace, facilitating personal loans, business loans, and financing of medical procedures. Borrowers can easily access lower interest rate loans through a fast online interface. 

 

Like most other lending companies, lending loans to ‘risky’ applicants is the largest source of financial loss (called credit loss). Credit loss is the amount of money lost by the lender when the borrower refuses to pay or runs away with the money owed. In other words, borrowers who default cause the largest amount of loss to the lenders. In this case, the customers labelled as 'charged-off' are the 'defaulters'. 

 

If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss. Identification of such applicants using EDA is the aim of this case study.

 

In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default.  The company can utilise this knowledge for its portfolio and risk assessment. 


To develop your understanding of the domain, you are advised to independently research a little about risk analytics (understanding the types of variables and their significance should be enough).

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
## Observations From Exploratory Data Analysis
#### Attributes to be looked into while Approving the Loan so that Loan would not be Defaulted-

* Term : Loan with term 36 months have higher Default percentage compared to 60 months.
* Grade: Loan with 'B' grade have higer percentage of default
* Sub Grade: Loan with Grade and subgrade 'B5' has higher percentage of default
* emp_length: Employees with experience more than 10 years have higher percentage of default. This might be because-
            a) As experience increases his/her age increases and other responsibilities might increase might result in default.
* home_ownership: People whole have a rented house defaulted more when compared to people who have Mortgaged their property or having own house.
                  This might be because people living in rent do not have much to lose. Others have their Home lost as part of recovery process
* verification_status: People whose incomes have been verified are very less prone to default. As their incomes are verified that means the values                          they quoted are correct and decision we have taken based on their income levels will be accurate.
* Purpose: People who takes loan for the purpose of debt consolidation are more prone to default. People who have more accounts opened are taking more loans/accounts to close other loans. In below figure we can observe the same.
* pub_rec: People with 0 public records are prone to higher number of defaulters.
* annual_income: People with annual income in range 27k-51k are prone to high default. From the derived metrics analysis of Monthly income to the installments we can observe - in this income group high percentage of the monthly income is going in installments which might be the reson for the high defaulters.
* revol_util: People with 40-60 % of revol_util are higher prone to Default
### Derived Metrics Observations

* Loans taken in the year 2011 are having higher defaulters. We can analyse more on this phenominon with supporting data to see the inflation rates and other metrics which could be the reason for the same.
* Loans taken in the month of December are having higher defaults.


<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
Python
Pandas
Numpy
matplotlib

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements



## Contact
Created by [satyateja100@githubusername] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
