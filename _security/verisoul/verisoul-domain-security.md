---
api_specs:
- filename: verisoul-account-api-openapi.yml
  format: yaml
  label: Verisoul Account API
  slug: verisoul-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-account-api-openapi.yml
- filename: verisoul-email-api-openapi.yml
  format: yaml
  label: Verisoul Email API
  slug: verisoul-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-email-api-openapi.yml
- filename: verisoul-enrollment-api-openapi.yml
  format: yaml
  label: Verisoul Enrollment API
  slug: verisoul-enrollment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-enrollment-api-openapi.yml
- filename: verisoul-list-api-openapi.yml
  format: yaml
  label: Verisoul List API
  slug: verisoul-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-list-api-openapi.yml
- filename: verisoul-phone-api-openapi.yml
  format: yaml
  label: Verisoul Phone API
  slug: verisoul-phone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-phone-api-openapi.yml
- filename: verisoul-public-api-openapi.yml
  format: yaml
  label: Verisoul Public API
  slug: verisoul-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-public-api-openapi.yml
- filename: verisoul-session-api-openapi.yml
  format: yaml
  label: Verisoul Session API
  slug: verisoul-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-session-api-openapi.yml
- filename: verisoul-verification-api-openapi.yml
  format: yaml
  label: Verisoul Verification API
  slug: verisoul-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisoul/refs/heads/main/openapi/verisoul-verification-api-openapi.yml
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
