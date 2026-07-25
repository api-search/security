---
api_specs:
- filename: opkit-benefits-api-openapi.yml
  format: yaml
  label: Opkit Benefits API
  slug: opkit-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-benefits-api-openapi.yml
- filename: opkit-eligibility-inquiries-api-openapi.yml
  format: yaml
  label: Opkit Eligibility Inquiries API
  slug: opkit-eligibility-inquiries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-eligibility-inquiries-api-openapi.yml
- filename: opkit-patients-api-openapi.yml
  format: yaml
  label: Opkit Patients API
  slug: opkit-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-patients-api-openapi.yml
- filename: opkit-payers-api-openapi.yml
  format: yaml
  label: Opkit Payers API
  slug: opkit-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-payers-api-openapi.yml
- filename: opkit-webhooks-api-openapi.yml
  format: yaml
  label: Opkit Webhooks API
  slug: opkit-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opkit.co
  spf: true
hosts:
- host: www.opkit.co
  https: false
- host: docs.opkit.co
  https: false
- host: api.opkit.co
  https: false
kind: domain-security
layout: security
method: probed
name: Opkit Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Opkit, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Opkit
provider_slug: opkit
slug: opkit-domain-security
source_filename: opkit-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.opkit.co\n  https: false\n- host: docs.opkit.co\n  https: false\n- host: api.opkit.co\n  https: false\ndomains:\n- domain: opkit.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/security/opkit-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Healthcare
- Insurance
- Eligibility
- Benefits
- Verification
- Telehealth
---
