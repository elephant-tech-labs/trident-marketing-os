# CRM Field Dictionary

| Field Name | Module | Type | Used For | Required? | Notes |
|---|---|---|---|---|---|
| Client type | Contacts | Picklist | Agent/Homeowner segmentation | Yes | Current master gate |
| First Name | Contacts | Text | Personalization | Yes | Merge: `$[UD:FIRST_NAME||]$` |
| Last Name | Contacts | Text | Form prefill | Optional | Merge: `$[UD:LAST_NAME||]$` |
| Contact Email | Contacts | Email | Email send/form prefill | Yes | Merge: `$[UD:CONTACT_EMAIL||]$` |
| Phone | Contacts | Phone | SMS/form prefill | Yes for SMS | Merge: `$[UD:PHONE||]$` |
| Address | Contacts | Text | Property-specific campaigns | Yes for homeowner workflows | Merge: `$[UD:ADDRESS||]$` |
| Last Inspection Date | Contacts | Date | Reactivation, trust anchor | Yes | Used carefully |
| Inspection Report Status | Inspection/Contacts | Picklist | Post-report workflow trigger | Recommended | Published is the entry event |
| Report Published At | Inspection/Contacts | DateTime | Post-report workflow timing anchor | Recommended | Use instead of appointment date for delays |
| Termite Inspection Date | Contacts | Date | Termite workflow | Recommended | Confirm merge field |
| WDO Findings | Contacts or Termite module | Picklist/Checkbox | Termite workflow eligibility | Recommended | Needed for better segmentation |
| Termite Treatment Booked | Contacts/Deal | Checkbox | Suppression/exit | Recommended | Suppress if true |
| Termite Treatment Completed | Contacts/Deal | Checkbox | Suppression/exit | Recommended | Suppress if true |
| Pest Plan Status | Contacts | Picklist | Pest suppression | Recommended | Active/Inactive/None |
| Email Opt-Out | Contacts | Checkbox | Suppression | Yes | Required |
| SMS Opt-Out | Contacts | Checkbox | SMS suppression | Yes | Required |
| SMS Consent | Contacts | Checkbox | SMS eligibility | Yes for SMS | Check again before every SMS send |
| Do Not Market | Contacts | Checkbox | Global suppression | Yes | Required |
| Agent Lifecycle Stage | Contacts | Picklist | Agent workflow routing | Recommended | New/Active/90D+/Dormant/VIP |
| Agent Sequence Status | Contacts | Picklist | Prevent overlap | Recommended | Not Started/Active/Paused/Completed |
| Pest Service Booked | Contacts/Deal | Checkbox | Pest workflow suppression and exit | Recommended | Stop automation when true |
| Pest Service Completed | Contacts/Deal | Checkbox | Pest workflow suppression and exit | Recommended | Stop automation when true |
| Active Marketing Workflow | Contacts | Picklist | Cross-workflow suppression | Recommended | Only one active marketing workflow |
| Active Complaint | Contacts/Desk | Checkbox | Global workflow suppression | Recommended | Stop all marketing follow-up when true |
