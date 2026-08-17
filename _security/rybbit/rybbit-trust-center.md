---
api_specs:
- filename: rybbit-analytics-api-openapi.yml
  format: yaml
  label: Rybbit Analytics API
  slug: rybbit-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-analytics-api-openapi.yml
- filename: rybbit-event-tracking-api-openapi.yml
  format: yaml
  label: Rybbit Event Tracking API
  slug: rybbit-event-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-event-tracking-api-openapi.yml
- filename: rybbit-sessions-api-openapi.yml
  format: yaml
  label: Rybbit Sessions API
  slug: rybbit-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/openapi/rybbit-sessions-api-openapi.yml
certifications: []
description: 'Rybbit publishes a security page describing visitor privacy protection, infrastructure, authentication, data ownership, deletion windows and compliance. It is a security/trust NARRATIVE, not a certification trust center: Rybbit holds no third-party security certification of its own, and there is no trust.rybbit.io / trust-portal surface.'
kind: trust-center
layout: security
name: Rybbit Trust Center
name_suffix: Trust Center
overview: Rybbit maintains a public trust center covering its security and compliance posture.
provider_name: Rybbit
provider_slug: rybbit
slug: rybbit-trust-center
source_filename: rybbit-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nprobe: false\nsource: https://rybbit.com/security\nurl: https://rybbit.com/security\ndescription: >-\n  Rybbit publishes a security page describing visitor privacy protection,\n  infrastructure, authentication, data ownership, deletion windows and\n  compliance. It is a security/trust NARRATIVE, not a certification trust\n  center: Rybbit holds no third-party security certification of its own, and\n  there is no trust.rybbit.io / trust-portal surface.\ncertifications: []\ncertifications_note: >-\n  CORRECTION (2026-08-13). Earlier rounds of this artifact listed \"ISO 27001,\n  PCI DSS, GDPR\" as Rybbit certifications. That was a keyword-match false\n  positive against this page: the ISO 27001 claim belongs to HETZNER, Rybbit's\n  hosting provider (\"Hetzner is ISO 27001 certified\"), and the PCI DSS claim\n  belongs to STRIPE, its payment processor (\"All payment processing is handled\n  by PCI DSS compliant payment processors\").\
  \ Rybbit itself states neither.\n  Attributing a vendor's certification to the provider overstates its posture,\n  so the list is now empty and the third-party certifications are recorded\n  separately below. Do not let the mechanical probe re-add them.\nthird_party_certifications:\n  - {holder: Hetzner, relationship: 'hosting provider (Germany, EU)', certification: ISO 27001}\n  - {holder: Stripe, relationship: payment processor, certification: PCI DSS}\n  - {holder: Cloudflare, relationship: R2 object storage for session replays, certification: none stated}\ncompliance_claims: [GDPR, CCPA, PECR]\ndpa: https://rybbit.com/dpa\nposture:\n  data_residency: Hetzner servers in Germany, within the European Union.\n  visitor_privacy:\n    - No cookies or local storage used for tracking.\n    - IP addresses hashed and anonymized.\n    - User-Agent strings hashed daily with rotating salts.\n    - Raw visitor data never stored.\n  network: Database servers are not reachable from the open internet;\
  \ private networks with firewall rules.\n  account_security:\n    - Passwords hashed and salted with a unique per-password salt.\n    - Sessions expire after 14 days of inactivity.\n  data_ownership:\n    - Customer owns 100% of their analytics data.\n    - Account, site and per-person deletion available.\n    - Analytics data permanently deleted within 60 days of cancellation.\n  transparency: Fully open source (AGPL-3.0), auditable by security researchers.\nevidence:\n  - source: https://rybbit.com/security\n    http_status: 200\n    fetched: '2026-08-13'\n    quotes:\n      - 'Hetzner is ISO 27001 certified'\n      - 'All payment processing is handled by PCI DSS compliant payment processors (Stripe).'\n      - 'GDPR compliant (no personal data collection)'\n      - 'CCPA compliant'\n      - 'PECR compliant (no cookie consent needed)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rybbit/refs/heads/main/security/rybbit-trust-center.yml
summary_line: trust center published
tags:
- Analytics
- Web Analytics
- Product Analytics
- Privacy
- Open Source
- Cookieless
trust_url: https://rybbit.com/security
---
