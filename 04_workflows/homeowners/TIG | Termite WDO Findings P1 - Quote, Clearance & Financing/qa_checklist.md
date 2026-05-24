# QA Checklist

## Segment QA
- [ ] Segment includes correct Client type
- [ ] Suppression rules applied
- [ ] Test contacts only used during QA
- [ ] No unsubscribed contacts included

## Merge Field QA
- [ ] First name renders correctly
- [ ] Address renders correctly where used
- [ ] Phone renders correctly
- [ ] Blank fallback tested
- [ ] No broken merge syntax

## Link QA
- [ ] CTA link works
- [ ] Form prefill works
- [ ] Source code is correct
- [ ] Phone link works on mobile
- [ ] Unsubscribe link works

## Email Design QA
- [ ] Gmail desktop checked
- [ ] Gmail mobile checked
- [ ] Outlook checked if possible
- [ ] Button visible
- [ ] Logo loads
- [ ] Footer address visible

## SMS QA
- [ ] Message includes opt-out if required
- [ ] Phone number is correct
- [ ] Reply keyword routing confirmed
- [ ] SMS send time is within acceptable hours

## Exit Rule QA
- [ ] Form submission exits workflow
- [ ] Booking exits workflow
- [ ] Reply creates task or notification
- [ ] STOP suppresses SMS
