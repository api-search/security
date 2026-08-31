---
api_specs:
- filename: origami-risk-authentication-api-openapi.yml
  format: yaml
  label: Origami Risk Authentication API
  slug: origami-risk-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-authentication-api-openapi.yml
- filename: origami-risk-hastokenexpired-api-openapi.yml
  format: yaml
  label: Origami Risk Has Token Expired API
  slug: origami-risk-hastokenexpired-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-hastokenexpired-api-openapi.yml
- filename: origami-risk-new-endpoint-1-api-openapi.yml
  format: yaml
  label: Origami Risk New Endpoint 1 API
  slug: origami-risk-new-endpoint-1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-new-endpoint-1-api-openapi.yml
- filename: origami-risk-new-endpoint-api-openapi.yml
  format: yaml
  label: Origami Risk New Endpoint API
  slug: origami-risk-new-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-new-endpoint-api-openapi.yml
- filename: origami-risk-requests-api-openapi.yml
  format: yaml
  label: Origami Risk Requests API
  slug: origami-risk-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/openapi/origami-risk-requests-api-openapi.yml
certifications: []
description: Origami Risk publishes a dedicated trust center on its own subdomain, https://trust.origamirisk.com/ (HTTP 200), hosted on Vanta. The report body is rendered client-side from Vanta's API, so the certification list, control set and document library are not readable anonymously from the served HTML — the page shell is all that is retrievable without the live client. No certification names are asserted here that were not verified on an Origami-controlled page.
kind: trust-center
layout: security
name: Origami Risk Trust Center
name_suffix: Trust Center
overview: Origami Risk maintains a public trust center covering its security and compliance posture.
provider_name: Origami Risk
provider_slug: origami-risk
slug: origami-risk-trust-center
source_filename: origami-risk-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nprobe: true\nsource: https://trust.origamirisk.com/\nurl: https://trust.origamirisk.com/\nplatform: Vanta Trust Center\ntitle: Origami Risk Trust Center\ndescription: >-\n  Origami Risk publishes a dedicated trust center on its own subdomain,\n  https://trust.origamirisk.com/ (HTTP 200), hosted on Vanta. The report body is\n  rendered client-side from Vanta's API, so the certification list, control set and\n  document library are not readable anonymously from the served HTML — the page shell\n  is all that is retrievable without the live client. No certification names are\n  asserted here that were not verified on an Origami-controlled page.\ncertifications: []\ncertifications_note: >-\n  Not enumerable from the anonymous fetch. The Vanta trust-report bundle loads its data\n  through an authenticated/JS-driven API; probes of the /api/v2/* paths return the SPA\n  HTML shell. Read the live trust center (or request access through it)\
  \ for the\n  current certification and document list.\ncompliance_claims_verified_on_origami_pages:\n- claim: HIPAA\n  source: https://www.origamirisk.com/solutions/grc/compliance-management/\n- claim: GDPR\n  source: https://www.origamirisk.com/privacy-policy/\n- claim: CCPA\n  source: https://www.origamirisk.com/privacy-policy/\nrelated_surfaces:\n- type: SLA\n  url: https://www.origamirisk.com/serviceterms/sla/\n  note: >-\n    Contractual 99.9% availability, service credits, and a documented backup regime\n    (15-minute incremental, nightly differential, weekly full, offsite to Amazon S3,\n    six-month weekly retention, periodic restore tests).\n- type: PrivacyPolicy\n  url: https://www.origamirisk.com/privacy-policy/\n- type: TermsOfService\n  url: https://www.origamirisk.com/origami-risk-website-terms-use/\n- type: AIGuidelines\n  url: https://www.origamirisk.com/platform/origami-risk-ai/ai-guidelines/\n- type: AIServiceTerms\n  url: https://www.origamirisk.com/serviceterms/aifeatures/\n\
  evidence:\n- source: https://trust.origamirisk.com/\n  status: 200\n  keywords:\n  - trust center\n  - vanta\n- source: https://www.origamirisk.com/serviceterms/sla/\n  status: 200\n  keywords:\n  - availability requirement\n  - service credits\n  - backup and recovery\nsuperseded:\n  previous_url: https://www.origamirisk.com/solutions/grc/compliance-management/\n  reason: >-\n    The automated probe first matched a GRC product page (Origami's compliance\n    management SOLUTION for customers), not Origami's own compliance posture. Replaced\n    2026-07-25 with the real first-party trust center.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/origami-risk/refs/heads/main/security/origami-risk-trust-center.yml
summary_line: trust center published
tags:
- Insurance
- United States
- Property and Casualty
- Policy Administration
- Claims
- Underwriting
- Core Systems
- Risk Management
- Workers Compensation
- Insurtech
- Billing
trust_url: https://trust.origamirisk.com/
---
