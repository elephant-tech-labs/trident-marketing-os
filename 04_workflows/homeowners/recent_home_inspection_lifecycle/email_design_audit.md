# Email Design Audit

Audit date: 2026-07-14

## Findings

The older pest campaign HTML should not be reused for recent inspection clients. It contains multiple brightly colored panels, gradients, emojis, urgency blocks, and repeated inline declarations. That presentation feels promotional and conflicts with the calm post-report strategy.

The existing global homeowner and pest base templates were placeholders. New campaigns therefore lacked a dependable, reusable email-safe foundation.

Some newer workflow HTML is cleaner, but several files include pasted Markdown fences inside the HTML and depend heavily on CSS classes. Campaign files must be clean HTML documents before import into Zoho.

The brand orange `#ffa201` does not provide sufficient contrast with white button text. The upgraded template uses dark navy text on orange for a clearer, more accessible CTA.

Historical campaign report exports contain recipient-level data. They were not changed during this design upgrade, but they should be removed from version control through a separate privacy cleanup because the repository policy prohibits customer PII.

## Design Decision

The recent-inspection campaign uses:

- 600-pixel hybrid email layout
- presentation tables and inline critical styles
- system fonts only
- one hosted Trident logo
- a personalized inspection-context block
- one primary CTA
- a plain reply/call/text alternative
- an Outlook-compatible VML button
- restrained brand color and no decorative imagery
- a reviewed plain-text companion for every email

## Deliverability Boundary

HTML cannot guarantee Primary Inbox placement. Authentication, consent, complaint rate, sending reputation, list quality, message relevance, and unsubscribe handling are more important than decorative design.

Current sender guidance:

- Google: https://support.google.com/mail/answer/81126
- Yahoo: https://senders.yahooinc.com/best-practices/
- Zoho custom HTML: https://help.zoho.com/portal/en/kb/campaigns/user-guide/email-campaigns/create-campaign/articles/how-to-import-html
- Zoho merge tags: https://help.zoho.com/portal/en/kb/campaigns/user-guide/settings/merge-tags/articles/predefined-merge-tags
