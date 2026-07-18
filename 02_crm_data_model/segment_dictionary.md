# Segment Dictionary

## TIG | Segment | Agents 90D+ Since Last Inspection

Criteria:
- Client type = Agent
- Last Inspection Date older than 90 days
- Email Opt-Out = false
- Do Not Market = false
- Agent Sequence Status != Active

Used by:
- TIG | Agent 90D+ Reactivation P1 - Keep Trident Handy

## TIG | Segment | Termite WDO Findings

Criteria:
- Client type = Homeowner
- Termite/WDO inspection = true
- WDO findings = yes
- Treatment booked = false
- Treatment completed = false
- Email Opt-Out = false
- Do Not Market = false

Used by:
- TIG | Termite WDO Findings P1 - Quote and Clearance

## TIG | Segment | Homeowners Pre-2025 Inspections

Criteria:
- Client type = Homeowner
- Last Inspection Date before 2025-01-01
- Pest Plan Status != Active
- Email Opt-Out = false
- Do Not Market = false

Used by:
- TIG | Pest Pre-2025 Activation P1 - Complimentary Pest Check

## TIG | Segment | Homeowners 2025 Inspections Pest Eligible

Criteria:
- Client type = Homeowner
- Last Home Inspection Date between 2025-01-01 and 2025-12-31
- Home Inspection Completed = true
- Pest Plan Status != Active
- Pest Service Booked != true
- Pest Service Completed != true
- Active Marketing Workflow = None
- Email Opt-Out = false
- Do Not Market = false

SMS Eligibility:
- Phone is not empty
- SMS Opt-Out = false

Used by:
- TIG | Pest 2025 Inspection Clients P1 - Seasonal Pest Check

## TIG | Segment | Recent Inspection Clients Pest Eligible

Criteria:
- Client type = Homeowner
- Inspection Report Status = Published
- Report Published At is not empty
- Home Inspection Completed = true
- Address is not empty
- Last Inspection Date is not empty
- Pest Plan Status != Active
- Pest Service Booked != true
- Pest Service Completed != true
- Active Marketing Workflow = None
- Email Opt-Out = false
- Do Not Market = false
- Active Complaint = false

SMS Eligibility:
- Phone is not empty
- SMS Consent = true
- SMS Opt-Out = false

Used by:
- TIG | Post-Report Pest Enrollment P1 - Recent Inspection Clients

Timing note:
- Report support begins on Day 1 after publication.
- Pest enrollment begins on Day 3 after publication.
