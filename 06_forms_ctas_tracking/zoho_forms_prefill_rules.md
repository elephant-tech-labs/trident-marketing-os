# Zoho Forms Prefill Rules

Recommended URL parameters:
- fname
- lname
- email
- phone
- address
- source

Example:
`?fname=$[UD:FIRST_NAME||]$&lname=$[UD:LAST_NAME||]$&email=$[UD:CONTACT_EMAIL||]$&phone=$[UD:PHONE||]$&address=$[UD:ADDRESS||]$&source=termite_wdo_e1`
