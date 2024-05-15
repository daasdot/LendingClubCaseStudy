# Lending Club Case Study
> You work for a consumer finance company which specialises in lending various types of loans to urban customers. When the company receives a loan application, the company has to make a decision for loan approval based on the applicant’s profile. Two types of risks are associated with the bank’s decision:

- If the applicant is likely to repay the loan, then not approving the loan results in a loss of business to the company

- If the applicant is not likely to repay the loan, i.e. he/she is likely to default, then approving the loan may lead to a financial loss for the company
  > In other words, the company wants to understand the driving factors (or driver variables) behind loan default, i.e. the variables which are strong indicators of default


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

<!-- You can include any other section that is pertinent to your problem -->

## General Information
> EDA involves analyzing and visualizing loan data to understand its key characteristics, uncover patterns, and identify relationships between variables refers to the method of studying and exploring record sets to apprehend their predominant traits, discover patterns, locate outliers, and identify relationships between variables
> The aim is to identify patterns which indicate if a person is likely to default, which may be used for taking actions such as Denying the loan,
Reducing the amount of loan. If one is able to identify these risky loan applicants, then such loans can be reduced thereby cutting down the amount of credit loss.Lending (to risky applicants) at a higher interest rate, etc.Identification of such applicants using EDA is the aim of this case study.

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- loan_amount
  >
   - loan_Amount has outliers post 30000 however looking at the data above 30000 , many applicants taken loan above 30000. So we can not tell these are outlier , but the values are quite high.
The distribution is positive skewed
- total_pymnt
  >
   - Total_pymnt has outliers post 35000 however looking at the data above 35000 , many applicants paid the total amount above 35000. So we can not tell these are outlier , but the values are quite high.
The distribution is positive skewed
- Annual Income
  >
    - Applicants with Higher salary has lesser chance to be charged_off.
    - Salary range between 0-20K has more chances of charged off.
    - As the salary grows the charge-off proportion goes down.
- employee length
  >
   - Applicant with No employement exprience or zero employment period has higher charged of propertion.
   - Looking at the data its difficult to deduce the impact of the emp_length on the charged off as the proportion are almost same.
- Grade
  >
   - Grade A employee has lower charged-off proportion.
   - Charged off proportion increases when the grade decreases. Lower the grade having higher charge-off proportion.
- purpose
  >
   - Small business has higher charged off proportion
   - Renewable_energy has lower charged off value compared to other.
- Interest Rate
  >
   - Higher the rate higher the charged-off proportion
   - Lower interest rate between 0-10 having lower charged off proportion
   - Higher rate more than 16 % will have higher charged of proportion
   - Nearly 70% of applicant have more than 10% interest which is also a high number.
   - 12.7 % having 16+ interest rate may have loan_status as charged_off
- DTI
  >
   - Low DTI are more attractive to loan approval
   - DTI above 15 may contain applicant with loan_status as charged off
- Address State
  >
   - State NE has higher of charged-off proportion.
   - FL , CA , NY have high charged off values.
- public bankrupcy record
  >
   - Applicant who has bankruppted they have more charged off proportion value. They falls into the chanrged off status.
   - Bankrupcy with value 2 has higher impact on the loan defaults.
- public record
  >
   - The applicants has legal debt-related matters they have higer charged off proportion. Have negative impact on the loan defaults.
   - Lender would have a risk to approve loan for those applicants.
- Term and int_rate has positive correlations
- Annual income and loan_amount has positive correlation
- dti and annual income has negative correlation
- Annual income and emp_length has positive correlation

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Technologies Used
- Python: version 3.x
- Pandas: version 1.3.4
- Seaborn: version 0.12.2
- Matplotlib: version 3.5.3
- Plotly: version 5.9.0

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->

## Acknowledgements
Give credit here.
- This project was inspired by the need to optimize the loan approval process and mitigate financial risks in consumer finance.


## Contact
Created by Dibya Ranjan Sethi - feel free to contact me!
