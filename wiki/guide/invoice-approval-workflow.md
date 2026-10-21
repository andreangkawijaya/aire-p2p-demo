---
type: guide
---
# Invoice Approval Workflow

## Standard Process

1. **Invoice received** — invoice registered against an open purchase order
2. **Three-way match** — quantities, unit prices, and totals compared across invoice, PO, and goods receipt
3. **Variance check** — variances above 2% or $500 (whichever is lower) are flagged for review
4. **Approval routing** — routed per the procurement policy thresholds
5. **Payment posting** — payment scheduled per the vendor's payment terms

## Exception Handling

- **Price variance** — if the invoice price differs from the PO price, the buyer must confirm the variance is accepted before payment
- **Quantity mismatch** — short receipts follow the received quantity; over-deliveries require a PO change
- **Missing goods receipt** — invoices without a goods receipt park in the exception queue for 24h, then auto-reject

## Fraud Prevention

Any request to skip the three-way match or bypass the approval threshold is a red flag. The CFO cannot pre-approve an invoice verbally — all approvals must flow through the system of record with a full audit trail.
