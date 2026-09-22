# 04. Cash Application

## Overview

Cash Application is the process of identifying customer payments and applying those receipts to the correct customer invoices.

It connects the collection activity with Accounts Receivable and ensures that customer accounts accurately reflect payments received.

## Cash Application Process

Customer Payment
↓
Payment Identification
↓
Customer Identification
↓
Invoice Matching
↓
Payment Application
↓
AR Balance Update
↓
Account Reconciliation

## Collection Register

| Receipt ID | Receipt Date | Customer | Invoice | Amount Received | Payment Method | Reference |
|---|---|---|---|---:|---|---|
| REC-001 | 25-Jan-2026 | C001 - Alpha Retail | INV-001 | ₹25,000 | Bank Transfer | BT-001 |
| REC-002 | 25-Feb-2026 | C003 - City Mart | INV-002 | ₹40,000 | Bank Transfer | BT-002 |
| REC-003 | 15-Mar-2026 | C002 - Beta Stores | INV-003 | ₹40,000 | Bank Transfer | BT-003 |
| REC-004 | 28-Mar-2026 | C004 - Daily Needs | INV-004 | ₹10,000 | Bank Transfer | BT-004 |

## Key Activities

### 1. Payment Identification

Payments received through the bank are reviewed and identified using information such as:

- Customer name
- Payment reference
- Bank transaction reference
- Payment amount
- Receipt date

### 2. Invoice Matching

The payment is matched against the appropriate customer invoice.

The matching process can use:

- Invoice number
- Customer ID
- Customer name
- Payment amount
- Bank reference

### 3. Payment Application

Once the payment is validated, it is applied against the outstanding invoice.

Example:

```text
Invoice Amount       ₹60,000
Payment Received     ₹40,000
Outstanding Balance  ₹20,000
