# Segment Rules

Zoho Campaigns Segment Name:

`TIG | Segment | Homeowners 2025 Inspections Pest Eligible`

## Required Criteria

* Client Type = Homeowner
* Last Home Inspection Date is between 2025-01-01 and 2025-12-31
* Home Inspection Completed = true
* Pest Plan Status != Active
* Pest Service Booked != true
* Pest Service Completed != true
* Active Marketing Workflow = None
* Email Opt-Out = false
* Do Not Market = false

## SMS Eligibility Criteria

For SMS steps, also require:

* Phone is not empty
* SMS Opt-Out = false

## Exclusions

Exclude contacts if:

* They have an active pest plan
* They already booked pest service
* They already completed pest service
* They are currently in a sales-active workflow
* They have an active complaint
* They opted out of email/SMS as applicable
* They are marked Do Not Market

## Notes

This segment is different from:

`TIG | Segment | Homeowners Pre-2025 Inspections`

The Pre-2025 segment should remain tied to homeowners inspected before 2025.

