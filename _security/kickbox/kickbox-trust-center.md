---
api_specs:
- filename: kickbox-account-api-openapi.yml
  format: yaml
  label: Kickbox Account API
  slug: kickbox-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-account-api-openapi.yml
- filename: kickbox-batch-api-openapi.yml
  format: yaml
  label: Kickbox Batch API
  slug: kickbox-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-batch-api-openapi.yml
- filename: kickbox-open-api-openapi.yml
  format: yaml
  label: Kickbox Open API
  slug: kickbox-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-open-api-openapi.yml
- filename: kickbox-verification-api-openapi.yml
  format: yaml
  label: Kickbox Verification API
  slug: kickbox-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-verification-api-openapi.yml
- filename: kickbox-disposable-api-openapi.yml
  format: yaml
  label: Kickbox Disposable API
  slug: kickbox-disposable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/openapi/kickbox-disposable-api-openapi.yml
certifications:
- SOC 2
- GDPR
- CCPA
description: ''
kind: trust-center
layout: security
name: Kickbox Trust Center
name_suffix: Trust Center
overview: Kickbox maintains a public trust center documenting SOC 2, GDPR, and CCPA compliance.
provider_name: Kickbox
provider_slug: kickbox
slug: kickbox-trust-center
source_filename: kickbox-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: false\nsource: https://docs.kickbox.com/docs/security-and-compliance\nurl: https://trust.kickbox.com/\nhttp_status: 200\nverified: '2026-08-13'\nsummary: >-\n  Kickbox operates a trust center at trust.kickbox.com, linked from its own Security and Compliance\n  documentation page with deep links into five control categories. The page itself is a JavaScript\n  single-page application and renders no server-side text, so the certification list below is taken\n  from Kickbox's documentation and pricing page rather than scraped from the trust center — the\n  mechanical probe (0-working/probe-security-programs.py) returned no hit for exactly that reason.\ncontrol_categories:\n  - {name: Infrastructure security, url: 'https://trust.kickbox.com/controls#infrastructure-security'}\n  - {name: Organizational security, url: 'https://trust.kickbox.com/controls#organizational-security'}\n  - {name: Product security, url: 'https://trust.kickbox.com/controls#product-security'}\n\
  \  - {name: Internal security procedures, url: 'https://trust.kickbox.com/controls#internal-security-procedures'}\n  - {name: Data and privacy, url: 'https://trust.kickbox.com/controls#data-and-privacy'}\ncertifications:\n  - name: SOC 2\n    status: claimed\n    note: >-\n      Kickbox makes two different claims about SOC 2 and both are recorded here rather than\n      reconciled. The docs page (Security and Compliance) invites readers to \"view our current\n      progress towards SOC2 compliance\" on the trust center, which reads as in-progress. The pricing\n      page states Kickbox \"is fully GDPR-compliant and SOC II certified\". No audit report or\n      attestation date is published on either page, so the status is recorded as claimed.\n    sources:\n      - https://docs.kickbox.com/docs/security-and-compliance\n      - https://kickbox.com/pricing\n  - name: GDPR\n    status: claimed-compliant\n    note: >-\n      \"We are GDPR compliant, following all of the EU's regulations for\
  \ data protection for our EU\n      customers.\" Kickbox operates dedicated EU verification servers and a separate EU application\n      (app.eu.kickbox.com / api.eu.kickbox.com).\n    docs: https://docs.kickbox.com/docs/gdpr\n    sources: [https://docs.kickbox.com/docs/security-and-compliance]\n  - name: CCPA\n    status: claimed-ready\n    note: Documented as \"CCPA and GDPR ready\".\n    sources: [https://docs.kickbox.com/docs/security-and-compliance]\nmemberships:\n  - name: M3AAWG\n    note: >-\n      Documented as membership in anti-abuse organizations \"like M3WAGG\" (the provider's own spelling\n      of M3AAWG, the Messaging, Malware and Mobile Anti-Abuse Working Group). Recorded verbatim from\n      the source with the intended organization noted.\n    sources: [https://docs.kickbox.com/docs/security-and-compliance]\ndata_handling:\n  - >-\n    Kickbox states it does not send email to verify addresses and does not accept customers who use\n    their lists for spam.\n  - >-\n\
  \    EU customers can have verifications processed on dedicated EU servers.\naccount_security:\n  - {feature: Sign in with Google, docs: 'https://docs.kickbox.com/docs/authentication-methods'}\n  - {feature: Two-factor authentication, docs: 'https://docs.kickbox.com/docs/authentication-methods'}\n  - {feature: Okta SSO, docs: 'https://docs.kickbox.com/docs/okta-authentication'}\nprivacy:\n  privacy_policy: https://docs.kickbox.com/docs/privacy-policy\n  subprocessors: https://docs.kickbox.com/docs/subprocessors\n  anti_spam_policy: https://docs.kickbox.com/docs/anti-spam-policy\n  list_security: https://docs.kickbox.com/docs/list-security-and-privacy\n  dsar_portal: https://privacyportal.onetrust.com/webform/f73513a8-7a10-4a9d-939a-703f8d994839/262761ab-edc4-440a-8e56-e6348b131382\nvulnerability_disclosure:\n  published: false\n  note: >-\n    Separately searched and not found. No /.well-known/security.txt on any Kickbox host, no\n    responsible-disclosure or bug-bounty page, and no HackerOne/Bugcrowd/Intigriti\
  \ program. The\n    mechanical probe returned vdp=none. No security/kickbox-vulnerability-disclosure.yml artifact and\n    no Security pointer are emitted — an honest absence.\n  evidence:\n    - {url: 'https://kickbox.com/.well-known/security.txt', status: 404}\n    - {url: 'https://kickbox.com/security.txt', status: 404}\n    - {url: 'https://api.kickbox.com/.well-known/security.txt', status: 404}\nevidence:\n  - {source: 'https://docs.kickbox.com/docs/security-and-compliance', status: 200, kind: provider-documentation}\n  - {source: 'https://trust.kickbox.com/', status: 200, kind: trust-center, note: JS-rendered; no server-side text}\n  - {source: 'https://kickbox.com/pricing', status: 200, kind: marketing-claim}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kickbox/refs/heads/main/security/kickbox-trust-center.yml
summary_line: SOC 2, GDPR, CCPA
tags:
- Email Verification
- Email Validation
- Deliverability
- Data Quality
- Email
trust_url: https://trust.kickbox.com/
---
