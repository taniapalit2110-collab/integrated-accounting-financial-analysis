# 03. Billing & Invoicing

## Overview

Billing and Invoicing is a core stage of the Order-to-Cash (O2C) process.

It converts completed sales orders into customer invoices and establishes the accounts receivable balance that must subsequently be collected.

## Billing Process

The billing flow can be represented as:

Sales Order
↓
Order Validation
↓
Invoice Creation
↓
Due Date Calculation
↓
Invoice Validation
↓
Customer Invoice
↓
Accounts Receivable

## Invoice Register

| Invoice ID | Invoice Date | Sales Order | Customer | Invoice Amount | Due Date | Amount Received | Outstanding | Status |
|---|---|---|---|---:|---|---:|---:|---|
| INV-001 | 10-Jan-2026 | SO-001 | C001 | ₹25,000 | 09-Feb-2026 | ₹25,000 | ₹0 | Paid |
| INV-002 | 18-Jan-2026 | SO-002 | C003 | ₹60,000 | 04-Mar-2026 | ₹40,000 | ₹20,000 | Partially Paid |
| INV-003 | 08-Feb-2026 | SO-003 | C002 | ₹40,000 | 10-Mar-2026 | ₹40,000 | ₹0 | Paid |
| INV-004 | 22-Feb-2026 | SO-004 | C004 | ₹30,000 | 24-Mar-2026 | ₹10,000 | ₹20,000 | Partially Paid |
| INV-005 | 05-Mar-2026 | SO-005 | C005 | ₹60,000 | 19-Apr-2026 | ₹0 | ₹60,000 | Outstanding |

## Key Billing Activities

### 1. Invoice Creation

Invoices are generated against valid sales orders.

Important invoice information includes:

- Invoice ID
- Invoice date
- Sales Order ID
- Customer ID
- Invoice amount
- Payment terms
- Due date
- Invoice status

### 2. Invoice Validation

Before releasing an invoice, key information should be checked:

- Customer details
- Sales order reference
- Quantity
- Pricing
- Invoice amount
- Payment terms
- Due date

### 3. Due Date Calculation

The invoice due date is determined using the customer's agreed payment terms.

For example:

```text
Invoice Date + Payment Terms = Due Date
