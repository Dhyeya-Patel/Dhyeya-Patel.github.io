# Payroll Reconciliation (Sample)

An Excel workbook that compares one pay period's **payroll register** to what was posted in the **general ledger (GL)** and flags differences to investigate.

> **All data is fictional.** No real company, employee, or payroll information is used. The workbook is a practice model of a reconciliation process.

## What's inside

| Tab | What it does |
|---|---|
| Payroll Register | 10 fictional employees with gross wages, withholdings, and employer taxes calculated by formula |
| GL Postings | What the books show for wages, employer payroll taxes, and employee withholdings |
| Reconciliation | Compares register vs. GL, shows the variance, and marks each line **Matches** or **Investigate** |

## What it finds

The sample GL has one built-in error: a bonus that was paid through payroll but never posted. The reconciliation catches it as a **$1,250 gross wages variance**, while employer taxes and withholdings match.

## How it works

- Tax amounts use simplified rates (Social Security 6.2%, Medicare 1.45%), stored in yellow assumption cells.
- Blue text is typed-in input, black text is a formula, green text pulls from another tab.
- Status uses a tolerance cell, so it can be tightened or loosened.

## Tools

Microsoft Excel (formulas: `SUM`, `ROUND`, `IF`, `ABS`, `COUNTIF`, cross-sheet references).

## What I learned

- Payroll register totals should match what is posted in the books.
- Here, wages were $1,250 lower in the books because one bonus was never posted. The other lines matched.
- The fix is an adjusting journal entry, and it's best to check this before closing the period.
