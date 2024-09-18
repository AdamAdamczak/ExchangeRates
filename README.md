# Currency Rates Automation Process

## Overview
This repository contains a UiPath automation project for fetching and processing currency exchange rates from the NBP website.

## Process Steps

### Fetch Currency Rates
- Retrieve the average exchange rates of foreign currencies (Table A) from the NBP website:
  - [NBP Currency Rates](https://www.nbp.pl/home.aspx?f=/kursy/arch_a.html)

### Create Excel Workbook
- Generate a new Excel workbook named `KursyWalut_yyyyMMdd.xlsx` (where `yyyyMMdd` is the current date).
- Create separate sheets for each currency: EUR, USD, CHF.

### Populate Data
- Extract and copy data from the fetched rates for the last 365 days into the corresponding sheets for each currency.

### Generate Line Charts
- For each currency, create a line chart in the respective sheet to visualize the exchange rate trends over the collected data period.

### Email Results
- Send the generated Excel file to the specified email address.
