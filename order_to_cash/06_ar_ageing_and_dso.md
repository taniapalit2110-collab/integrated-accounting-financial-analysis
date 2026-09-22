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
