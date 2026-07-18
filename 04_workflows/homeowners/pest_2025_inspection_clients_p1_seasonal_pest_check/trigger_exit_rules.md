# Trigger and Exit Rules

## Trigger

Contact enters the campaign when they match:

`TIG | Segment | Homeowners 2025 Inspections Pest Eligible`

## Start Conditions

* Contact is not already in another active workflow
* Contact has completed a home inspection in 2025
* Contact is pest eligible
* Contact is not opted out
* Contact is not marked Do Not Market

## Exit If

Exit immediately if any of the following happen:

* Contact replies with pest interest
* Contact replies requesting a call
* Contact submits pest booking form
* Contact submits callback form
* Pest deal is created
* Pest service is booked
* Pest service is completed
* Pest plan becomes Active
* Contact opts out
* SMS STOP received
* Do Not Market becomes true
* Active complaint is created
* Contact becomes Sales Active / Human Follow-Up

## CRM Updates on Exit

If form submitted or reply intent is positive:

* Active Marketing Workflow = Sales Active / Human Follow-Up
* Current Homeowner Marketing Segment = Pest Inquiry
* Last Campaign Response = Pest 2025 Inspection Clients
* Create/update Pest Deal
* Create Work Queue item or Desk ticket depending on operating setup

If campaign completes without response:

* Active Marketing Workflow = None
* Marketing Workflow Status = Completed
* Next Eligible Campaign = Homeowner Monthly Property Care

