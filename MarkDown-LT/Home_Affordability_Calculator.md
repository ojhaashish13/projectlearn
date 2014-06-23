# Home Affordability Calculator

## Overview

Home Affordability Calculator helps user to understand how much home amount user can afford based on his income and other debts. This module has two parts:

### Home Affordability Calculator
When the user taps Home Affordability Calculator option it opens Home Affordability calculation screen. Using this calculator user can calculate total amount which can be affordable to the user to buy a home. There are three types of affordability:
 
* Conservative
* Moderate
* Aggressive

Following fields are required to calculate Home Affordability of the user:

* Annual Income ($30,000 to $990,000)
* Down Payment ($0 to $1,00,000)
* Mortgage Rate (2% to 7.25%)
* Monthly Debts (Customized)


Assumptions are things which are taken into consideration. these assumptions are as follows:

* Annual Property Taxes (Default value is 1.140%)
* Annual Homeowner's Insurance (Default value is $800)
* Annual HOA Dues (Default value is $0)
* Loan Term in Years (Default value is 30)
* Private Mortgage Insurance - PMI (Default value is On)


### Amortization Details

This page shows amortization details according to the inputs given by the user in the previous(Calculator) screen. When user taps "Details" button on Navigation Bar it opens Amortization view. It shows Home Affordability break-up details to user with payment details on monthly basis for selected loan terms.


## Code Base

Code for Home Affordability Calculator Module resides in following classes / screens

### Home Affordability Calculator

* LTMortgageInformationViewController

### Amortization Details

* LTMortgageAffordabilityAmortizationViewController


## Calculation Part

Calculation part code for Home Affordability Calculator Module resides in following screens / classes

* HomeAffordabilityData

* * *

© 2014 V2solutions. All rights reserved.