# Bond Service Interview Assignment

## Objective
Your task is to create a backend service for a corporate bond investment app using Python, Django, and Django Rest Framework. This system will allow users to manage their corporate bond investments and track performance over time.

## Features
### 1. User Authentication
Simple API token authentication is sufficient.

### 2. Bond Management
Users should be able to:
- Add new bonds to their portfolio, including the issue name, issue ISIN, bond value, coupon rate, purchase date, maturity date, and frequency of interest payments.
- Update the details of the bonds they own.
- Delete a bond from their portfolio.
- View a list of all the bonds they own.

### 3. Investment Analysis
Implement an endpoint that returns an analysis of the user's portfolio, including:
- Average coupon rate across all bonds.
- The bond that will mature next.
- Total value of the portfolio.
- Future value of portfolio

### 4. API Documentation
Include an API documentation using Django Rest Framework's built-in tools or a third-party package.

### 5. Validations
ISIN should be validated against Central Security Depository public API. Here’s the example API call with a valid ISIN identifier:
```
GET https://www.cdcp.cz/isbpublicjson/api/VydaneISINy?isin=CZ0003551251

{
   "vydaneisiny":[
      {
         "cval":"CZ0003551251",
         "ison":"Rentico Invest/11.23 DEB 20260531",
         "tval":"100",
         "pdcp":"list",
         "regdt":"2023-05-24",
         "eico":"0019319703",
         "ename":"Rentico Invest s.r.o.",
         "elei":"315700PZ559GOUR26559"
      }
   ]
}
```
### 6. Tests
Write a reasonable amount of tests.

### NTH: 7. Dockerize Django backend

## We'll be looking at
- Well-structured and clean code
- Application of RESTfull API principles
- Error handling
- Testing approach

## Submission
Please host the code in a GitHub repository. Include a README file with instructions on how to set up and run the project.

