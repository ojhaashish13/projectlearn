# Mortgage Payment Calculator

## Overview

Mortgage Payment Calculator can help estimate your monthly mortgage payments, including estimates for taxes, insurance and PMI. This module has two parts:

### Mortgage Calculator

When the user taps Mortgage Payment Calculator option it opens Mortgage Calculation screen. Using this calculator user can calculate total monthly mortgage payment based on entered Home Price Amount, Down Payment, Mortgage Rate, Loan Terms and some pre-define assumption like Property Tax etc, whose values can be change. Following fields are required to calculate Mortgage Payment:
 
* Home Price ($50,000 to $2,00,000)
* Down Payment (0% to 100%)
* Mortage Rate (2% to 7.5%)

Assumptions are things which are taken into consideration. These assumptions are as follows:

* Annual Property Taxes (Default value is 1.140%)
* Annual Homeowner's Insurance (Default value is $800)
* Annual HOA Dues (Default value is $0)
* Loan Terms in Years (Default value is 30)
* Private Mortgage Insurance - PMI (Default value is Off)


### Amortization Details

This page shows amortization details according to the inputs given by the user in the previous(Calculator) screen. When user taps "Details" button on Navigation Bar it opens Amortization view. It shows mortgage break-up details to user with mortgage payment details on monthly basis for selected loan terms.


## Code Base

Code for Mortgage Payment Calculator Module resides in following classes / screens

### Mortgage Calculator

* LTMortgagePaymentViewController

### Amortization Details

* LTMortgageAmortizationViewController


## Calculation Part

Calculation part code for Mortgage Payment Calculator Module resides in following screens / classes

* MortgageData.h

* * *

© 2014 V2solutions. All rights reserved.


