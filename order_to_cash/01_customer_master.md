# 01. Customer Master

## Overview

The Customer Master is the foundation of the Order-to-Cash (O2C) process.

It contains the key information required to identify customers, determine payment terms, manage credit exposure, and support accurate billing and collections.

## Customer Master Data

| Customer ID | Customer Name | Customer Type | Payment Terms | Credit Limit |
|-------------|---------------|---------------|---------------|--------------|
| C001 | Alpha Retail | Retail | 30 Days | ₹150,000 |
| C002 | Beta Stores | Retail | 30 Days | ₹125,000 |
| C003 | City Mart | Wholesale | 45 Days | ₹200,000 |
| C004 | Daily Needs | Retail | 30 Days | ₹100,000 |
| C005 | Metro Traders | Wholesale | 45 Days | ₹250,000 |

## Key Fields

### Customer ID
A unique identifier assigned to each customer.

### Customer Name
The legal or business name used for customer identification and billing.

### Customer Type
Classifies customers, such as:

- Retail
- Wholesale

### Payment Terms
Defines the agreed period within which the customer is expected to make payment.

Examples:

- 30 Days
- 45 Days

### Credit Limit
Represents the maximum approved credit exposure for the customer.

## O2C Importance

Customer Master data supports:

- Accurate invoice creation
- Correct payment-term assignment
- Credit control
- Accounts receivable management
- Collections prioritisation
- Customer account reconciliation

## Controls

Important controls include:

- Unique customer IDs
- Valid customer information
- Approved payment terms
- Credit-limit validation
- Customer master review
- Prevention of duplicate customer records

## Excel Skills Demonstrated

The accompanying Excel workbook uses lookup logic to connect customer IDs with customer names and other master-data attributes.

Example:

```excel
=INDEX('Customer Master'!B2:B6,MATCH(C2,'Customer Master'!A2:A6,0))
