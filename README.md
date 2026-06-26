# Loan Payoff Calculator

A simple, self-contained HTML page that calculates a loan amortization schedule and lets you edit the inputs live.

## Files

- `loan-payoff-table.html` — the calculator. Open it in any web browser; no server or internet connection required.

## What it does

Given:
- **Loan amount** ($)
- **Interest rate** (APR %)
- **Monthly payment** ($)

It calculates:
- Number of months to pay off the loan
- Total interest paid
- Total amount paid (principal + interest)
- A full month-by-month table showing payment, interest, principal, and remaining balance

## How it works

Interest accrues monthly using `monthly rate = APR / 12`, applied to the remaining balance. Each payment first covers that month's interest, with the rest going toward principal. The final payment is automatically reduced to whatever payoff amount remains.

## Usage

1. Open `loan-payoff-table.html` in a browser (double-click the file, or drag it into a browser window).
2. Edit any of the three input fields — the summary cards and table recalculate automatically.
3. If the monthly payment is too low to cover the monthly interest, the page will show a warning instead of an infinite table.

## Notes

- This assumes a fixed monthly payment and a fixed APR for the life of the loan (standard amortizing loan behavior).
- It does not account for variable rates, fees, or extra one-time payments.
- All calculations run locally in the browser — no data is sent anywhere.
