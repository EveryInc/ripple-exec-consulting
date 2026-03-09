# Contract & PO Reviewer

## Prompt

I'm SVP of Marketing and Communications at Ripple. I sign and approve dozens of vendor contracts and purchase orders every week for events, comms agencies, news subscriptions, venues, PR firms, and more. I also get a lot of fraudulent invoices and POs. I need a tool that helps me quickly triage these.

Using the attached `sample_contracts.csv` and `sample_purchase_orders.csv`, build me a tool that:

1. **Reads each contract/PO** and produces a structured summary:
   - Vendor name and contact info
   - Contract type (services, subscription, event, venue, agency retainer, etc.)
   - Total value and payment terms
   - Key dates (start, end, renewal, cancellation deadline)
   - Auto-renewal clause (yes/no - flag if yes)
   - Liability and indemnification summary
   - Unusual or non-standard terms (flagged in red)
   - IP/content ownership terms (critical for marketing/comms contracts)

2. **Fraud/Red Flag Scanner** - For each document, check for:
   - Vendor not in approved vendor list
   - Bank details that don't match known vendor records
   - Duplicate invoice/PO numbers
   - Pricing significantly above market rate
   - Missing standard clauses (termination, data privacy, NDA)
   - Suspicious urgency language ("payment required within 24 hours")
   - Mismatched company names or addresses

3. **Decision Recommendation** - For each contract/PO, output one of:
   - APPROVE - standard terms, known vendor, fair pricing
   - REVIEW - some non-standard terms that need attention (list them)
   - ESCALATE - significant red flags detected (list them)
   - REJECT - likely fraudulent or clearly non-compliant

Output as a clean HTML report I can quickly scan, with the most important information front and center. Color-code by recommendation (green/yellow/orange/red).
