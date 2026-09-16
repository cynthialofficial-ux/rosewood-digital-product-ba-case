# 05 — UAT and Release Readiness

## UAT approach

The BA owns traceability from business intent to testable outcomes and coordinates business acceptance; QA remains responsible for formal test execution appropriate to the delivery model.

### Sample critical UAT cases

- Editorial CTA opens the correct property booking context.
- Dates and party information persist where valid.
- Returning-guest profile failure falls back to manual checkout.
- Marketing consent remains unselected unless previously and validly captured.
- AEM blocks publication when required content is incomplete.
- Mobile preview has no critical layout / content issue.
- Booking-service timeout retains user inputs and presents a recovery path.
- Funnel analytics fires exactly once with approved non-PII attributes.

## Defect triage model

**P1** — Booking blocked, wrong reservation context, privacy/security risk, materially incorrect price/policy display.  
**P2** — Major journey degradation with workaround, important content or localisation defect.  
**P3** — Minor visual/content issue with no material business or guest impact.

## Go / no-go gates

1. No Must-have story without approved acceptance criteria.
2. No unresolved P1 defect.
3. P1 UAT coverage executed and evidenced.
4. AEM content complete for pilot properties and approved by Brand / property owner.
5. Integration recovery paths tested.
6. Core funnel analytics validated in test.
7. Named operational support owners and escalation route confirmed.

## Release follow-up

- 24–48 hour defect / incident review.
- One-week funnel and content-quality check.
- Property / business-user feedback capture.
- Backlog update for optimisation and A/B-test opportunities.
