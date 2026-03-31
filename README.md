# 📊 ACME Company Accounting System

> A fully automated Excel-based double-entry accounting system for small businesses.
> Enter transactions once and watch all financial reports update automatically.

---

## 🧾 What This Project Is

This is a formula-driven accounting system built entirely in Microsoft Excel for ACME Company.
It covers the full accounting cycle — from journal entry to financial statements — with no
manual calculations required.

---

## 💡 Why It Was Built

Most small businesses and students cannot afford professional accounting software like QuickBooks or Sage.
This project was built to solve that problem by creating a transparent, automated accounting system in Excel that:

- ✅ Teaches double-entry bookkeeping in a practical way
- ✅ Automates financial reporting from a single data entry point
- ✅ Enforces data consistency using dropdown validation
- ✅ Shows the full accounting cycle from journal entry to financial statements
- ✅ Helps small business owners track cash, expenses, liabilities and profit at no software cost

---

## 🔧 What Problem It Solves

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

## 📂 Sheets Included

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

## ⚡ Key Features

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

## 📋 Chart of Accounts

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

## 🚀 How to Use

1. Open `Accounting system.xlsx`
2. Go to the `Transactions` sheet
3. Enter journal entries starting from row 4:
   - Select Account from the dropdown
   - Enter Date, Description, Debit or Credit (enter 0 for the other), Due Date
   - Type `Paid` in column H when a transaction is completed
   - Leave Status column (G) empty — it calculates automatically
4. Every journal entry needs **TWO rows** — one debit and one credit
5. Both rows of the same entry must have the **SAME date**
6. Press **F9** to refresh all formulas after entry
7. Review Trial Balance, Income Statement, Balance Sheet and Dashboard

---

## 📁 Project Files

| File | Purpose |
|---|---|
| `Accounting system.xlsx` | The Excel workbook |
| `README.md` | Project summary |

---

## ⚠️ Notes

- Each journal entry must have equal debits and credits
- Account names must be selected from the dropdown — do not type manually
- Press F9 if values appear stale or not updating
- To add new accounts go to Chart of Accounts and add a new row, then extend report rows accordingly

---

## 🛠️ Built With

![Microsoft Excel](https://img.shields.io/badge/Microsoft_Excel-217346?style=for-the-badge&logo=microsoft-excel&logoColor=white)
