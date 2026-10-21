# Finance OS Demo

A working demonstration of a monthly close for an early-stage SaaS company.

## The problem
Startups and software companies run on many different systems:
- CRM (Salesforce, HubSpot, etc.)
- Billing (Stripe, Chargebee, etc.)
- Accounting (QuickBooks, Xero, NetSuite)
- Banking
- Spend tools (Ramp, Brex, etc.)
- Payroll

These systems export data in different formats. Customer IDs do not match. Amounts are formatted differently. Dates vary. Some records are duplicated or incomplete. The result is inconsistent, unstructured data that someone has to clean and reconcile before the numbers can be trusted.

Most early-stage teams still do this work manually in spreadsheets. It is slow, error-prone, and produces numbers that live in different places.

## What this workflow does
1. Takes the messy exports from those systems
2. Normalizes and structures the data
3. Applies deterministic rules that are unique to each company  
   (These rules must be customized. They encode how *that* company defines ARR, matches customers, maps expenses, and reconciles the bank. This is the most important step — without the company’s own rules, the system cannot produce trusted numbers.)
4. Engages an agent only when the rules cannot handle an item cleanly
5. Requires human approval
6. Produces one trusted snapshot

That snapshot creates a holistic picture of the business:
- What is happening with the customer base
- How actuals compare to plan
- What the cash position and runway look like

## Why I am building this
AI makes it practical to automate the repetitive parts of the close without giving up control.

Once the company’s rules are set up:
- The system cleans and structures the data the same way every month
- Deterministic rules handle the majority of matching, classification, and reconciliation automatically
- An agent investigates only the edge cases
- A human still approves before anything is trusted

This saves time on the manual cleanup that currently dominates the close. It also improves accuracy and consistency — the same rules are applied every month, and every number traces back to an approved snapshot instead of a one-off spreadsheet.

Accurate, trusted numbers matter because they drive real decisions:
- How to allocate capital
- Which marketing strategies are working and which are not (including ROI on marketing spend through cohort analysis)
- Whether the company can afford new hires and how those hires affect profitability and burn
- How the business is tracking against plan
- When capital needs to be raised and how much runway remains

Without a reliable close, these decisions are made on incomplete or conflicting data. The goal of this workflow is to produce one trusted set of numbers so the company can make those decisions with confidence.

The first setup requires work (capturing the company’s definitions and mappings). After that, the monthly process is mostly review of exceptions.

## How to run
1. Download the HTML file from this repo
2. Open it in a browser
3. Click **Start guided demo**

The company and data are synthetic (Acme AI). The workflow is the point.

## Status
Working demo. Still evolving.
