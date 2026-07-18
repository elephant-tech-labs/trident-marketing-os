# QA Checklist

## Copy and Offer

- [ ] No report finding or issue is referenced
- [ ] No termite, WDO, rodent, infestation, pricing, or plan-name language appears
- [ ] Copy does not assume ownership or closing
- [ ] Offer says the first service is complimentary only if service begins
- [ ] CTA does not imply the pest check is free unless that is operationally true

## Personalization

- [ ] First name renders correctly
- [ ] Property address renders correctly
- [ ] Inspection date renders in a natural client-facing format
- [ ] Empty-field fallbacks remove the full affected phrase
- [ ] No unknown or generic template tags remain

## Email Rendering

- [ ] Gmail desktop and mobile checked
- [ ] Apple Mail desktop and mobile checked
- [ ] Outlook desktop checked
- [ ] Yahoo Mail checked where possible
- [ ] Logo loads with useful alt text
- [ ] CTA remains visible when images are blocked
- [ ] Mobile layout has no horizontal scrolling
- [ ] Dark mode remains readable
- [ ] Plain-text version is reviewed in Zoho

## Deliverability

- [ ] SPF, DKIM, and DMARC alignment verified for the sending domain
- [ ] Reply-To inbox is monitored
- [ ] Zoho one-click unsubscribe headers are enabled where required
- [ ] Exactly one visible Zoho unsubscribe link is present
- [ ] Physical business address is present
- [ ] Booking link uses an approved, recognizable domain
- [ ] No public URL shortener is used
- [ ] Campaign volume is increased gradually if the sending pattern is new

## Automation

- [ ] Entry is anchored to Report Published At
- [ ] Existing pest clients are excluded
- [ ] Positive replies beyond the exact PEST keyword are recognized
- [ ] Questions and positive replies stop the automation
- [ ] Booking, complaint, opt-out, and human follow-up stop the automation
- [ ] SMS consent is checked before every SMS
