---
api_specs:
- filename: verisoul-session-openapi.json
  format: json
  label: Verisoul Session API
  slug: verisoul-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-session-openapi.json
- filename: verisoul-account-openapi.json
  format: json
  label: Verisoul Account API
  slug: verisoul-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-account-openapi.json
- filename: verisoul-list-openapi.json
  format: json
  label: Verisoul Lists API
  slug: verisoul-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-list-openapi.json
- filename: verisoul-phone-openapi.json
  format: json
  label: Verisoul Phone API
  slug: verisoul-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-phone-openapi.json
- filename: verisoul-email-openapi.json
  format: json
  label: Verisoul Email Intelligence API
  slug: verisoul-email-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-email-openapi.json
- filename: verisoul-email-batch-openapi.json
  format: json
  label: Verisoul Email Intelligence Batch API
  slug: verisoul-email-intelligence-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-email-batch-openapi.json
- filename: verisoul-idcheck-openapi.json
  format: json
  label: Verisoul ID Check API
  slug: verisoul-id-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-idcheck-openapi.json
- filename: verisoul-facematch-openapi.json
  format: json
  label: Verisoul Face Match API
  slug: verisoul-face-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-facematch-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: verisoul.ai
  spf: true
hosts:
- cert_expires: Oct  2 20:04:09 2026 GMT
  host: www.verisoul.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 06:23:05 2026 GMT
  host: docs.verisoul.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 07:43:51 2026 GMT
  host: api.prod.verisoul.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Verisoul Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verisoul, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Verisoul
provider_slug: verisoul
slug: verisoul-domain-security
source_filename: verisoul-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.verisoul.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:04:09 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.verisoul.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 06:23:05 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.prod.verisoul.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 07:43:51 2026 GMT\n  hsts: null\ndomains:\n- domain: verisoul.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/security/verisoul-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fraud Detection
- Identity Verification
- Fake Account Detection
- Device Fingerprinting
- Email Intelligence
- Bot Detection
- KYC
- Trust and Safety
- Risk Scoring
---
