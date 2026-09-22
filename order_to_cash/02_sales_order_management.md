# 02. Sales Order Management

## Overview

Sales Order Management is an important stage of the Order-to-Cash (O2C) lifecycle.

It captures customer orders and provides the foundation for downstream billing, invoicing, accounts receivable, and collections activities.

## Sales Order Data

| Sales Order ID | Order Date | Customer | Product / Service | Quantity | Unit Price | Order Value | Status |
|---|---|---|---|---:|---:|---:|---|
| SO-001 | 05-Jan-2026 | C001 - Alpha Retail | Laptop Accessories | 10 | ₹2,500 | ₹25,000 | Invoiced |
| SO-002 | 12-Jan-2026 | C003 - City Mart | Networking Equipment | 5 | ₹12,000 | ₹60,000 | Invoiced |
| SO-003 | 03-Feb-2026 | C002 - Beta Stores | Office Equipment | 8 | ₹5,000 | ₹40,000 | Invoiced |
| SO-004 | 18-Feb-2026 | C004 - Daily Needs | Printer Supplies | 20 | ₹1,500 | ₹30,000 | Partially Paid |
| SO-005 | 02-Mar-2026 | C005 - Metro Traders | IT Hardware | 4 | ₹15,000 | ₹60,000 | Outstanding |

## Key Activities

### 1. Order Capture

Record customer orders with:

- Sales Order ID
- Order date
- Customer ID
- Product or service
- Quantity
- Unit price
- Order value
- Order status

### 2. Order Validation

Before billing, key information should be validated, including:

- Customer details
- Product or service
- Quantity
- Pricing
- Payment terms
- Order status

### 3. Order-to-Invoice Linkage

Each sales order should be linked to the corresponding customer invoice.

This provides traceability across the O2C process:

**Sales Order → Invoice → Payment → Accounts Receivable**

## Order Value Calculation

The order value can be calculated using:

```excel
Quantity × Unit Price
Example:

=E6*F6

For SO-001:

10 × ₹2,500 = ₹25,000
Customer Lookup

Customer information can be retrieved from the Customer Master using a lookup formula.

Example:

=INDEX('Customer Master'!B2:B6,MATCH(C6,'Customer Master'!A2:A6,0))

This retrieves the customer name based on the Customer ID.

Order Status Monitoring

The model uses order statuses such as:

Invoiced
Partially Paid
Outstanding

Monitoring these statuses helps identify orders requiring downstream billing or collection action.

O2C Controls

Key controls include:

Unique sales order numbers
Customer validation
Price and quantity validation
Order-value verification
Sales-order-to-invoice linkage
Order status monitoring
Business Importance

Accurate sales order management helps ensure:

Correct billing
Reduced invoice disputes
Better revenue tracking
Complete transaction traceability
Faster downstream collections
Portfolio Demonstration

This section demonstrates practical understanding of how sales orders flow into billing and ultimately into Accounts Receivable and collections.

Note: The transactions and financial values used in this portfolio are illustrative and created for demonstration purposes only.
