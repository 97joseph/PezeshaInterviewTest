# PezeshaInterviewTest
Project Solution

# PezeshaInterview
 Interview Solution

# Task: 1

Develop a REST API that implements a simple money transfer between accounts feature.

The API should have the following endpoints:

POST /accounts: creates a new account with a starting balance.

GET /accounts/{id}: retrieves the account information.

POST /transfers: transfers money from one account to another.

The API should have the following constraints:

An account can't have a negative balance.

The transfer amount must be greater than zero.

If the source account doesn't have enough funds, the transfer should fail.

The API should be able to handle concurrent requests and avoid race conditions.

The implementation should use a relational database (such as PostgreSQL) to store the accounts information and transactions.

Criteria for Evaluation:


API functionality: The API should meet all the requirements and constraints specified above.

Code quality: The code should be clean, readable, and well-organized. It should follow best practices for backend development and include appropriate comments.

Scalability and performance: The API should be scalable and perform well under heavy load.

Security: The API should be secure and prevent common web vulnerabilities such as SQL injection and cross-site scripting (XSS).

DevOps: The API should be easily deployable in a production environment and include appropriate logging and monitoring.

You can use any programming language and framework that you feel comfortable with. The API should be delivered along with the source code and a detailed README file that explains how to build and run the API, as well as any additional information that you consider relevant.

Please submit the code via a link to a public repository in a Git hosting platform like GitHub, GitLab, or Bitbucket.


# Task: 2

Write a function that implements a loan repayment calculator.

The loan repayment calculator should take the following input parameters:

Loan amount

Loan term (in months)

Interest rate (per year)

Repayment frequency (monthly, bi-monthly, or weekly)



The loan repayment calculator should output the following information:

Total interest to be paid over the loan term

Total amount to be repaid over the loan term

A table showing the breakdown of the loan repayments over the loan term, including the principal and interest amounts, and the remaining balance after each repayment.

Assume that the interest is calculated based on the outstanding balance of the loan, and that repayments are applied first to the interest and then to the principal.

Criteria for Evaluation:


Correctness: The output of the function should be correct and consistent with the input parameters.

Performance: The function should perform well for large inputs, taking into consideration time and space complexity.

Code quality: The code should be clean, readable, and well-organized. It should follow best practices for software development and include appropriate comments.

Test coverage: The code should include appropriate test cases to demonstrate the correct behavior of the function.


You can use any programming language and framework that you feel comfortable with. The solution should be delivered along with the source code and a detailed README 

file that explains how to build and run the code, as well as any additional information that you consider relevant.

Please submit the code via a link to a public repository in a Git hosting platform like GitHub, GitLab, or Bitbucket.

