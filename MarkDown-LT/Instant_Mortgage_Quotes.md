# Instant Mortgage Quotes

## Overview

### Loan View

When the user taps Instant Mortgage Quotes option it opens Loan View screen.

#### Loan Purpose

Using this screen user can select the purpose of his loan. There are two options available among which user has to select only one:
 
* Purchase
* Refinance

By default "Purchase" option is selected.


#### Type Of Home

After selecting Loan Purpose user will get navigated to this screen where he has to select type of home he want to buy. There are four options available among which user has to select only one:

* Single Family
* Town Home
* Condo
* Multi-Family

By default "Single Family" option is selected.

#### Home Use

After selecting Type of Home user will get navigated to this screen where he has to select user of his home. There are three options available among which user has to select only one:

* Primary Home
* Secondary Home
* Investment Property

By default "Primary Home" option is selected.

#### Estimated Home Value

After selection of Home Use screen user will get navigated to this screen where he has to enter estimated home value between $50,000 to $2,00,000.

#### Down Payment

After entering the estimated home value at "Estimated Home Value" screen user will get navigated to this screen where he has to enter amount of down payment between 0% to 100%.

#### How's Your Credit

After entering down payment user will get navigated to this screen where he has to rate his credit. There are four credit options available among which user has to select only one:

* Excellent (If credit is greater than 720)
* Good (If credit is between 680 and 719)
* Fair (If credit is between 640 and 679)
* Not So Good (If credit is below 639)

#### Property Zip Code

After selction of Credit Level user will get navigated to this screen where he has to enter the zip code of the property.
After entering zip code user can click "Get Offers" button on the same screen.

### Resulting Loan Offers

After Clicking "Get Offers" button from the Property Zip Code screen user will get navigated to this screen where a list of available loan offers will get displayed as per user preferences.

### Filter Your Results

Available loan offers can be filtered and sort in this screen. User can apply filters on:

* Loan Type
* Sort By
* Points

### Review Of Result

This screen shows reviews of the available loan offer.

### Details Of Result

This screen shows details of the selected loan offer.

## Code Base

Code for Instant Mortgage Quotes Module resides in following classes / screens:

### Loan View

* LTLoanViewController

### Resulting Loan Offers

* LTResultViewController

### Filter Loan Offers

* LTFilterViewController

### Review Of Result

* LEReviewViewController

### Details Of Results

* LTLenderDetailViewController


## Calculation Part

Calculation part code for Instant Mortgage Quotes Module resides in following screens / classes:

* LTLoanExplorerAPI
* LTLenderReviewsAPI
* LTEmailToLenderAPI

* * *

© 2014 V2solutions. All rights reserved.


