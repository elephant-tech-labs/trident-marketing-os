# QA Checklist

## Segment QA

* [ ] Segment name is correct: `TIG | Segment | Homeowners 2025 Inspections Pest Eligible`
* [ ] Client Type = Homeowner
* [ ] Last Home Inspection Date is between 2025-01-01 and 2025-12-31
* [ ] Home Inspection Completed = true
* [ ] Pest Plan Status != Active
* [ ] Pest Service Booked != true
* [ ] Pest Service Completed != true
* [ ] Active Marketing Workflow = None
* [ ] Email Opt-Out = false
* [ ] Do Not Market = false
* [ ] SMS steps suppress SMS opt-outs

## Asset QA

* [ ] Email subject lines do not imply confirmed pest issues
* [ ] Copy uses seasonal/property-care framing
* [ ] CTA links are final
* [ ] Source codes are correct
* [ ] UTM parameters are correct
* [ ] Unsubscribe link is present
* [ ] Physical address is present
* [ ] SMS includes opt-out language

## Automation QA

* [ ] Positive reply exits workflow
* [ ] Form fill exits workflow
* [ ] Pest deal creation exits workflow
* [ ] Pest service booked exits workflow
* [ ] Pest plan active exits workflow
* [ ] Active complaint exits workflow
* [ ] Do Not Market exits workflow
* [ ] STOP updates SMS Opt-Out

## CRM / Work Queue / Desk QA

* [ ] Pest inquiry creates or updates Contact
* [ ] Pest inquiry creates Pest Deal
* [ ] Pest inquiry creates Work Queue item or Desk ticket
* [ ] Source code captured
* [ ] Campaign response captured
* [ ] Contact moves to Sales Active / Human Follow-Up

