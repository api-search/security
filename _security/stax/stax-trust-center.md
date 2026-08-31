---
api_specs:
- filename: stax-api-openapi.json
  format: json
  label: Stax API
  slug: stax-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stax/refs/heads/main/openapi/stax-api-openapi.json
certifications: []
description: ''
kind: trust-center
layout: security
name: Stax Trust Center
name_suffix: Trust Center
overview: Stax maintains a public trust center covering its security and compliance posture.
provider_name: Stax
provider_slug: stax
slug: stax-trust-center
source_filename: stax-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: probed\nsource: https://trust.staxpayments.com/\nurl: https://trust.staxpayments.com/\nstatus: 200\nplatform: Laika (laika-app-prod.s3.amazonaws.com/static/trust-center)\ncertifications_readable: false\ncertifications: []\nnote: 'A trust center exists on Stax''s own subdomain and returns 200 with <title>Trust Center</title>, but the response body\n  is an 814-byte single-page-app shell: the entire content loads from a Laika-hosted JavaScript bundle. No certification name,\n  attestation date or document list is present in the served HTML, so nothing machine-readable can be recorded here. The only\n  certification Stax states in readable form is PCI DSS Level 1 Service Provider, captured in conformance/stax-conformance.yml.'\nchecked: '2026-08-29'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stax/refs/heads/main/security/stax-trust-center.yml
summary_line: trust center published
tags:
- Payments
- Payment Processing
- Merchant Services
- Embedded Payments
- ACH
- Invoicing
- Subscription Billing
- Surcharging
- Point of Sale
- Tokenization
- Financial Services
- Fintech
- Card Present
- Merchant Onboarding
trust_url: https://trust.staxpayments.com/
---
