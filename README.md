# Global Salary Calculator

A simple salary calculator for checking what an international job offer looks like after currency conversion and estimated taxes.

I made this mainly for comparing salaries across countries without having to manually calculate everything each time.

**Live Demo:** [Global Salary Calculator](https://global-salary-calculator.vercel.app)

## What it does

You enter:

- Original currency
- Annual salary

That's it.

The calculator then shows:

- Annual salary in the original currency
- Annual salary in INR
- Monthly gross salary
- Monthly gross salary in INR
- Estimated tax/deductions
- Annual take-home salary
- Monthly take-home salary
- Take-home salary in INR

The take-home figures are shown as **low, high, and average estimates**, since the actual amount depends on the person's tax situation.

## Supported currencies

Currently supported:

- USD — US Dollar
- SGD — Singapore Dollar
- EUR — Euro
- GBP — British Pound
- CAD — Canadian Dollar
- AUD — Australian Dollar
- CHF — Swiss Franc
- JPY — Japanese Yen
- AED — UAE Dirham
- NZD — New Zealand Dollar

## How to use

Select the currency and enter the annual salary.

For example:

**Currency:** USD  
**Annual Salary:** 100000

The calculator will then calculate the monthly salary, convert the figures to INR, apply the estimated tax range, and show the approximate take-home amount.

## How it calculates

The basic calculations are:

```text
Monthly Salary = Annual Salary / 12

INR Salary = Original Salary × Exchange Rate
```

For take-home pay, the calculator uses a minimum and maximum estimated tax/deduction percentage for each currency.

This produces three estimates:
1. Low
2. High
3. Average

The aim is to give a quick idea of the salary rather than provide an exact tax calculation.

Tech used: HTML, CSS, JavaScript

There are no frameworks or external dependencies. The application runs directly in the browser.

## Running locally
1. Clone the repository:
```bash
git clone https://github.com/SreeEswaran/global-salary-calculator.git
```
2. Then open index.html in your browser.
3. For an idea you can view the live demo as well.
4. 
That's all you need.

## Note
The tax percentages and exchange rates are approximate and intended for general comparison. Actual take-home salary can vary based on tax residency, deductions, state/province, social-security contributions, and other individual factors.

Exchange rates also change over time, so the values used in the calculator may need to be updated.

## Future improvements
1. More countries and currencies
2. Live exchange rates
3. More detailed country-specific tax calculations
4. Cost-of-living comparison
5. Comparing multiple job offers
6. Salary comparison charts
