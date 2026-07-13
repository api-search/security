---
api_specs:
- filename: opkit-openapi.yml
  format: yaml
  label: Opkit Eligibility Inquiries API
  slug: eligibility-inquiries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-openapi.yml
- filename: opkit-openapi.yml
  format: yaml
  label: Opkit Benefits API
  slug: benefits
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-openapi.yml
- filename: opkit-openapi.yml
  format: yaml
  label: Opkit Payers API
  slug: payers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-openapi.yml
- filename: opkit-openapi.yml
  format: yaml
  label: Opkit Patients API
  slug: patients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-openapi.yml
- filename: opkit-openapi.yml
  format: yaml
  label: Opkit Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opkit/refs/heads/main/openapi/opkit-openapi.yml
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
