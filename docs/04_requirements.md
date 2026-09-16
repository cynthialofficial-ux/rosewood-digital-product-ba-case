# 04 — Requirements, Stories and Dependencies

## Example epic: Context continuity

### RW-101 — Preserve destination context

**User story**  
As a guest arriving from editorial content, I want destination and stay context preserved when I enter booking so I do not restart my journey.

**Acceptance criteria**

1. **Given** a valid property context exists, **when** the guest selects Reserve, **then** the booking journey opens with the correct property context.
2. **Given** valid dates and party information exist, **when** the booking journey opens, **then** those values are retained and remain editable.
3. **Given** the passed context is missing or invalid, **when** booking opens, **then** a clear editable fallback is shown rather than a technical error.
4. The context handoff must not expose sensitive guest data in the URL or analytics payload.

## Example epic: Guest profile and consent

### RW-104 — Permission-based profile reuse

**User story**  
As a returning guest, I want my permitted profile details reused so I can complete forms faster without losing control of marketing consent.

**Acceptance criteria**

1. Profile details are reused only where the required permission / identity state exists.
2. Marketing consent is not preselected when consent has not been recorded.
3. A profile-service failure never blocks manual checkout.
4. Error logging contains no sensitive guest data.

## Example epic: AEM content readiness

### RW-105 — Structured content validation

**User story**  
As a content editor, I want structured AEM fields and validation rules so rooms, dining, wellness and experience content publishes consistently across properties.

**Acceptance criteria**

1. Required fields block publish when missing.
2. CTA type is restricted to approved action / destination types.
3. Editors can preview approved desktop and mobile states.
4. Localised content follows agreed fallback rules.

## Non-functional requirements

- Accessibility: keyboard flow, labels, focus and error messaging considered in acceptance.
- Performance: context persistence must not materially degrade booking-start performance.
- Privacy: no PII in analytics events or URL parameters.
- Resilience: manual paths remain available when profile or ancillary integrations fail.
- Localisation: content and policy variation must be supported by market / property.
- Observability: critical integration failures produce actionable monitoring events.

## Publicly evidenced vs assumed tools

**Publicly evidenced in Rosewood digital roles:** AEM, Jira, Confluence, Agile delivery, UAT, external vendors, A/B testing.

**Modelled generically in this case:** CRS / booking service, guest-profile / CRM service, analytics platform. Current production vendors are not assumed unless Rosewood publicly confirms them.
