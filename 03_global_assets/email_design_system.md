# Email Design System

## Core Principle

Trident email should feel like a useful continuation of a real service relationship. Design supports recognition and comprehension; it should not make a client feel that they entered a generic promotional funnel.

## Technical Baseline

- Use a complete HTML document with a doctype, language, charset, and viewport.
- Use a 600-pixel hybrid table layout with `width="100%"` and `max-width:600px`.
- Use presentation tables for layout and inline all critical styles.
- Use Arial, Helvetica, or another system-safe font stack.
- Do not depend on JavaScript, forms, iframes, video, external CSS, web fonts, gradients, or background images.
- Include an Outlook-compatible VML fallback for the primary button.
- Keep useful alt text on every meaningful image.
- Include a short hidden preheader followed by spacing characters.
- Include a reviewed plain-text version in Zoho.
- Keep HTML comfortably below Gmail clipping thresholds.

## Brand Tokens

| Purpose | Value |
| --- | --- |
| Primary accent | `#ffa201` |
| Headline / button text | `#0a2540` |
| Body text | `#334155` |
| Muted text | `#64748b` |
| Soft context background | `#f5f7fa` |
| Border | `#dfe5eb` |
| Footer | `#0f172a` |

Use dark navy text on the orange CTA. White text on Trident orange does not provide enough visual contrast.

## Layout Hierarchy

1. Logo and sender recognition
2. Short, literal headline
3. Personalized relationship context
4. Concise service explanation
5. One primary CTA
6. Reply/call/text alternative
7. Human signature
8. Physical address and one visible unsubscribe link

## Homeowner Emails

- Use property address and inspection date when they establish legitimate relevance.
- Keep the content column calm and mostly white.
- Use no more than one highlighted context or offer block.
- Use one primary button and one plain-language secondary response path.
- Avoid pest imagery when the client has not reported or confirmed a pest issue.

## Recent Inspection Emails

- Report delivery and report support must not contain a pest offer.
- Pest enrollment begins in a separate message after the approved delay.
- The inspection-context block should confirm the property and date without implying a report finding.
- Do not assume that the transaction closed.
- Use `the property` rather than `your new home`.

## Agent Emails

- Use a clean B2B letter style.
- Keep brand graphics minimal.
- Use one subtle orange accent and one clear contact action.

## Termite/WDO Emails

- Use a serious, restrained layout.
- Use report context as the trust anchor only for correctly segmented contacts.
- Use calm urgency and never amplify fear.

## Deliverability Rules

- HTML cannot guarantee Primary Inbox placement.
- Keep marketing and transactional messages in appropriately separated sending streams.
- Verify SPF, DKIM, DMARC, TLS, sender alignment, and monitored Reply-To configuration.
- Enable provider-supported one-click unsubscribe headers and keep one visible Zoho unsubscribe link in the body.
- Use recognizable HTTPS destinations and avoid public URL shorteners.
- Do not place customer PII in public query-string parameters.
- Keep subject lines accurate and consistent with message content.
- Send only to eligible, consented contacts and suppress bounces, complaints, and opt-outs promptly.

## Required QA

- Preview and send tests from Zoho, not only a browser.
- Check Gmail, Apple Mail, Outlook desktop, Outlook web, and Yahoo where possible.
- Test desktop, narrow mobile, image blocking, dark mode, long addresses, and missing merge fields.
- Verify that every campaign has a valid plain-text alternative.
- Verify the CTA destination, source code, unsubscribe link, physical address, and monitored reply path.
