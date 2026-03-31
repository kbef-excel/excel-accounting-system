# ACME Company Accounting System

## What This Project Is
This is a fully automated Excel-based accounting system built for ACME Company.
It allows a user to enter journal transactions once and have all financial reports
update automatically — General Ledger, Trial Balance, Income Statement, Balance Sheet and Dashboard.

---

## Why This Project Was Built
Most small businesses and students cannot afford professional accounting software like QuickBooks or Sage.
This project was built to solve that problem by creating a transparent, formula-driven accounting system
entirely in Microsoft Excel that:
- teaches double-entry bookkeeping in a practical way
- automates financial reporting from a single data entry point
- enforces data consistency using dropdown validation
- shows the full accounting cycle from journal entry to financial statements
- helps small business owners track cash, expenses, liabilities and profit without any software cost

---

## What Problem It Solves
| Problem | Solution |
|---|---|
| Manual posting of journal entries | Transactions sheet auto-posts to all reports |
| Repeated calculations for reports | SUMIF formulas calculate automatically |
| Account name typos breaking reports | Dropdown validation from Chart of Accounts |
| Wrong sign for account balances | VLOOKUP checks Normal Balance column |
| No visibility into overdue payments | Status column auto-calculates from Due Date |
| Balance sheet not balancing | Balance Check formula shows Balanced or Not Balanced |
| No summary view | Dashboard pulls key metrics from all sheets |

---

## Sheets Included

| Sheet | Purpose |
|---|---|
| `Chart_of_Accounts` | Defines all account codes, names, types and normal balances |
| `Transactions` | Journal entry input — the only sheet you type data into |
| `General_Ledger` | Mirrors transactions and shows account balances per row |
| `Trial_Balance` | Totals debits and credits per account and checks they balance |
| `Income_Statement` | Shows revenue, expenses and net income |
| `Balance_Sheet` | Shows assets, liabilities and equity in professional format |
| `Dashboard` | Summary of key totals and balance status |
| `Instructions` | How to use the workbook |

---

## Key Features
- Automated formulas using `SUMIF` and `VLOOKUP`
- Normal Balance column in Chart of Accounts drives correct balance signs
- Income Statement structured with Revenue and Expenses sections and Net Income
- Balance Sheet structured as Statement of Financial Position with Non-Current and Current sections
- Data validation on Transactions for Account (dropdown), Date, Due Date and Paid columns
- Status column auto-calculates as Pending or Overdue based on Due Date
- Manual Paid override column (H) in Transactions
- Balance Check on Trial Balance and Balance Sheet
- Dashboard references all report sheets for live summary

---

## Chart of Accounts
| Code | Account | Type | Normal Balance |
|---|---|---|---|
| 1001 | Cash | Asset | Debit |
| 1002 | Bank | Asset | Debit |
| 1003 | Accounts Receivable | Asset | Debit |
| 1004 | Inventory | Asset | Debit |
| 1005 | Equipment | Asset | Debit |
| 1006 | Land | Asset | Debit |
| 1007 | Buildings | Asset | Debit |
| 1008 | Machinery | Asset | Debit |
| 2001 | Accounts Payable | Liability | Credit |
| 2002 | Notes Payable | Liability | Credit |
| 3001 | Capital | Equity | Credit |
| 3002 | Retained Earnings | Equity | Credit |
| 4001 | Sales Revenue | Revenue | Credit |
| 4002 | Service Revenue | Revenue | Credit |
| 5001 | Rent Expense | Expense | Debit |
| 5002 | Utilities Expense | Expense | Debit |
| 5003 | Salaries Expense | Expense | Debit |
| 5004 | Supplies Expense | Expense | Debit |

---

## How to Use
1. Open `Accounting system.xlsx`
2. Go to the `Transactions` sheet
3. Enter journal entries starting from row 4:
   - Select Account from the dropdown
   - Enter Date, Description, Debit or Credit (enter 0 for the other), Due Date
   - Type `Paid` in column H when a transaction is completed
   - Leave Status column (G) empty — it calculates automatically
4. Every journal entry needs TWO rows — one debit and one credit
5. Both rows of the same entry must have the SAME date
6. Press **F9** to refresh all formulas after entry
7. Review Trial Balance, Income Statement, Balance Sheet and Dashboard

---

## Project Files
| File | Purpose |
|---|---|
| `Accounting system.xlsx` | The Excel workbook |
| `sample_transactions.md` | Sample transactions to enter as reference |
| `README.md` | Project summary |
| `learning_guide.md` | Accounting concepts and how to learn from this project |
| `interview_questions_answers.md` | Interview Q&A and possible exam questions |
| `Accounting system formulas explanation.md` | All formulas explained with purpose |

---

## Expected Results After Entering Sample Transactions
| Account | Balance |
|---|---|
| Cash | 4,550.00 |
| Accounts Receivable | 1,800.00 |
| Service Revenue | 3,800.00 |
| Accounts Payable | 300.00 |
| Capital | 5,000.00 |
| Rent Expense | 1,000.00 |
| Utilities Expense | 250.00 |
| Salaries Expense | 1,200.00 |
| Supplies Expense | 300.00 |
| Net Income | 2,250.00 |

---

## Notes
- Each journal entry must have equal debits and credits
- Account names must be selected from the dropdown — do not type manually
- Press F9 if values appear stale or not updating
- To add new accounts go to Chart of Accounts and add a new row, then extend report rows accordingly
