# 03 — Discovery-to-Booking Journey

## Primary guest journey

| Stage | Guest need | Digital behaviour | BA focus |
|---|---|---|---|
| Discover | Be inspired by a place and experience | Reads editorial / destination / hotel content | Entry context, content metadata, CTA rules |
| Consider | Understand property and stay options | Views rooms, offers and experiences | Content consistency, dependencies, availability handoff |
| Configure | Set dates, party and preferences | Starts reservation flow | State persistence, validation, recoverability |
| Select | Compare room / rate options | Reviews rate and room choices | Business rules, policy display, back-navigation state |
| Checkout | Complete reservation confidently | Enters guest details and consent | Privacy, consent, validation, error handling |
| Confirm | Know reservation succeeded | Receives confirmation | Confirmation data, analytics, support path |
| Curate stay | Add relevant experiences | Explores dining, wellness and experiences | Property relevance, handoff, operational readiness |

## To-be principle

**Do not make the guest repeatedly reconstruct intent that the experience already knows.**

That means preserving valid context where permitted, while always allowing the guest to edit it and always providing a graceful fallback when an upstream integration is unavailable.

## Business-user journey

The portfolio also treats content editors and property teams as users. A globally scalable digital product fails if AEM authors cannot publish confidently or if properties cannot fulfil what the website promises.

Key business-user requirements therefore include:

- required content fields and validation;
- mobile / desktop preview;
- localisation and fallback rules;
- explicit property ownership for experience details;
- UAT participation and escalation ownership;
- launch communications and support guidance.
