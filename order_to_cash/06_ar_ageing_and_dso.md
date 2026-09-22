# 06. AR Ageing & DSO

## Overview

Accounts Receivable (AR) Ageing is used to classify outstanding customer invoices according to the number of days they have remained unpaid.

Ageing analysis helps Finance and Collections teams identify overdue balances, prioritise collection activities, and monitor credit exposure.

Days Sales Outstanding (DSO) is a key O2C metric used to measure the average time taken to collect customer receivables.

## AR Ageing Process

Outstanding Invoices
↓
Due Date Validation
↓
Days Outstanding Calculation
↓
Ageing Bucket Classification
↓
Overdue Balance Identification
↓
Collections Prioritisation
↓
Management Reporting

## Ageing Buckets

| Ageing Bucket | Description |
|---|---|
| Not Yet Due | Invoice payment date has not yet been reached |
| 0–30 Days | Outstanding for up to 30 days |
| 31–60 Days | Outstanding for 31–60 days |
| 61–90 Days | Outstanding for 61–90 days |
| 90+ Days | Outstanding for more than 90 days |

## O2C Ageing Example

| Invoice | Customer | Outstanding | Days Outstanding | Ageing Bucket |
|---|---|---:|---:|---|
| INV-002 | C003 - City Mart | ₹20,000 | 27 | 0–30 Days |
| INV-004 | C004 - Daily Needs | ₹20,000 | 7 | 0–30 Days |
| INV-005 | C005 - Metro Traders | ₹60,000 | 0 | Not Yet Due |

## Days Outstanding

Days outstanding can be calculated by comparing the reporting date with the invoice due date.

Conceptually:

```text
Days Outstanding = Reporting Date - Invoice Due Date
For invoices that are not yet due, the ageing value should not be treated as overdue days.

Outstanding Receivables

Total outstanding Accounts Receivable is calculated by adding the unpaid balances of customer invoices.

Example:

INV-002    ₹20,000
INV-004    ₹20,000
INV-005    ₹60,000
-------------------
Total      ₹100,000
Ageing Analysis

Ageing analysis helps identify:

Current receivables
Overdue receivables
High-value outstanding invoices
Collection priorities
Potential credit-risk areas
Customer payment patterns
Days Sales Outstanding (DSO)

DSO measures the average number of days required to collect Accounts Receivable.

A commonly used formula is:

DSO = Average Accounts Receivable / Credit Sales × Number of Days

For example, using a 365-day period:

DSO = Average AR / Annual Credit Sales × 365

A consistent DSO calculation should use a clearly defined reporting period and matching sales and receivables data.

Why DSO Matters

DSO is useful for monitoring:

Collection efficiency
Working capital
Customer payment behaviour
Cash-flow performance
Credit-control effectiveness

Changes in DSO should be investigated together with ageing trends, customer mix, disputes, and payment terms.

Collections Prioritisation

Ageing information can support collection prioritisation.

Examples:

High-value overdue invoices
Long-outstanding balances
Repeatedly overdue customers
Invoices approaching significant ageing thresholds
Disputed invoices requiring resolution
Excel Reference

The practical implementation is available in:

order_to_cash.xlsx

Relevant worksheets:

Invoice Register
O2C Ageing
O2C Dashboard

These worksheets demonstrate outstanding balance tracking, ageing classification, and O2C management reporting.

Controls

Key AR ageing controls include:

Correct invoice due dates
Accurate payment application
Regular ageing refresh
Reconciliation to the AR ledger
Review of overdue balances
Investigation of ageing exceptions
Consistent ageing-bucket definitions
Business Importance

AR ageing and DSO analysis help Finance teams:

Improve collection planning
Identify overdue receivables
Manage working capital
Support cash-flow forecasting
Monitor collection performance
Provide management visibility
Portfolio Demonstration

This section demonstrates how transaction-level Accounts Receivable data can be transformed into ageing analysis and collection-focused management information.

Note: The transactions and financial values used in this portfolio are illustrative and created for demonstration purposes only.
