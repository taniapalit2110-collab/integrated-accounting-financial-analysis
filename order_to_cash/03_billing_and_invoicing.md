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
For a customer with 30-day payment terms:

10-Jan-2026 + 30 Days = 09-Feb-2026
4. Outstanding Balance

The outstanding balance represents the amount still due from the customer.

Formula:

=Invoice Amount - Amount Received

Example:

=F6-G6

For INV-002:

₹60,000 - ₹40,000 = ₹20,000
Invoice Status

The model uses the following statuses:

Paid
Partially Paid
Outstanding

These statuses provide visibility into the current collection position.

Accounting Impact

When an invoice is generated, the typical accounting entry is:

Accounts Receivable     Dr
       Revenue                 Cr

When the customer makes payment:

Bank / Cash              Dr
       Accounts Receivable      Cr

This creates a clear accounting flow from billing through cash collection.

O2C Controls

Key billing controls include:

Unique invoice numbers
Sales-order-to-invoice linkage
Pricing validation
Duplicate invoice checks
Due-date validation
Invoice amount verification
Customer master validation
Outstanding balance reconciliation
Excel Reference

The practical implementation of this process is available in:

order_to_cash.xlsx

Relevant worksheet:

Invoice Register

The workbook demonstrates invoice tracking, payment application, outstanding balance calculation, and invoice-status monitoring.

Business Importance

Accurate billing helps:

Reduce invoice disputes
Prevent revenue leakage
Improve cash collection
Maintain accurate Accounts Receivable
Support timely month-end reporting
Improve customer experience
Portfolio Demonstration

This section demonstrates practical understanding of the transition from sales order processing to billing and Accounts Receivable management.

Note: The transactions and financial values used in this portfolio are illustrative and created for demonstration purposes only.
