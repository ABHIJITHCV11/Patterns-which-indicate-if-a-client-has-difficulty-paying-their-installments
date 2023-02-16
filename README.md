
# Identification of risky applicants using EDA

This case study aims to identify patterns which indicate if a client has difficulty paying their installments

[Untitled.ipynb](https://github.com/ABHIJITHCV11/eda2/blob/master/Untitled.ipynb) *Contains the python code.*

[Presentation 4.pdf](https://github.com/ABHIJITHCV11/eda2/blob/master/Presentation%204.pdf) *Contains Overall approach of the analysis,key findings and conclusions.*
 


## 1. Problem statement
The loan providing companies finds it hard to give loans to the people due to their 
insufficient or non-existent credit history. Because of that, some consumers use it as their 
advantage by becoming a defaulter. Suppose you work for a consumer finance company 
which specializes in lending various types of loans to urban customers. You have to use 
EDA to Analyse the patterns present in the data. This will ensure that the applicants 
capable of repaying the loan are not rejected .

## 2. Risks associated with the bank’s decision

When the company receives a loan application,
the company has to decide for loan approval based on the applicant’s profile. 
Two types of risks are associated with the bank’s decision:

• If the applicant is likely to repay the loan, 
then not approving the loan results in a loss of business to the company

• If the applicant is not likely to repay the loan, i.e. he/she is likely to default, 
then approving the loan may lead to a financial loss for the company.


## 3. Scenarios

**The data contains the information about the loan application at the time of 
applying for the loan. It contains two types of scenarios:** 

• The client with payment difficulties: he/she had late payment more than X days on at least 
one of the first Y instalments of the loan in our sample,

• All other cases: All other cases when the payment is paid on time.

**When a client applies for a loan, there are four types of decisions that could 
be taken by the client/company):**

• Approved: The Company has approved loan Application

• Cancelled: The client cancelled the application sometime during approval. 
Either the client changed her/his mind about the loan or in some cases due to a higher 
risk of the client he received worse pricing which he did not want.

• Refused: The company had rejected the loan 
(because the client does not meet their requirements etc.).

• Unused offer:  Loan has been cancelled by the client but on different stages of the process.

 ## 4. Data
 
 **This dataset has 3 files as explained below:** 

 

1. ['application_data.csv'](application_data.csv)  contains all the information of the client at the time of application.
The data is about whether a client has payment difficulties.

2. ['previous_application.csv'](previous_application.csv) contains information about the client’s previous loan data. It contains the data whether the previous application had been Approved, Cancelled, Refused or Unused offer.

3. ['columns_description.csv'](columns_description.csv) is data dictionary which describes the meaning of the variables.

## 5. Business Objectives
This case study aims to identify patterns which indicate if a client has dif ficulty paying 
their installments which may be used for taking actions such as denying the loan, reducing 
the amount of loan , lending (too risky applicants) at a higher interest rate, etc . This will 
ensure that the consumers capable of repaying the loan are not rejected . Identification of 
such applicants using EDA is the aim of this case study.

## 6. Overall approach of the analysis
The files are captured , understood , prepared for analysis (cleaned , processed) and
analyses via different methods (statistical summaries and plotting). Then some conclusions
are drawn based on the results.

[Untitled.ipynb](https://github.com/ABHIJITHCV11/eda2/blob/master/Untitled.ipynb) *Contains the python code.*

[Presentation 4.pdf](https://github.com/ABHIJITHCV11/eda2/blob/master/Presentation%204.pdf) *Contains Overall approach of the analysis,key findings and conclusions.*

## 6. Conclusion
### Distribution
- 92% of people didn't default whereas to 8% defaulted.
- From the above statistics it is clear that the data is imbalanced
- We can't predict if a person is a defaulter just by looking at their SALARY
- The salary distrubution of defaulter's and defaulter's are very close
- This means we can not directly predict if a person will be defaulter or not, just by looking at their salary

### Gender discripancy findings
- 57 % of defaulters are females.
- But we have to remeber, 65 % of loans were took by females.Thus they have more defaulters.
- Also, from our analysis it is clear that percentage of male defaulters are high compared to females.

### Does owning a car make a difference ?
- 34 % of non-defaulters own a car while only 30 % of defaulters own it.
- But there are about 2 times more people that does not own a car compared to people that own a car.
- Thus owning a car makes Not much difference

### Loans .
- Unemployed and Maternity leave loan takes have the highest percentage of defaulters in their group respectively.
- Students and Businessman have 100 % non default rate(But very few of them took loans).
- old_senior_citizen's (70+) do not take loans
- for non defaulter's senior_cityzen's are found to take more loans
- for defaulter's adult's are found to take more loans
- Features that can contribute in predicting target feature NAME_EDUCATION_TYPE,AMT_INCOME_TOTAL,DAYS_BIRTH,AMT_CREDIT,DAYS_EMPLOYED,AMT_ANNUITY
