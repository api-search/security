---
api_specs:
- filename: credentially-gateway-openapi-original.json
  format: json
  label: Credentially Public API
  slug: credentially-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credentially/refs/heads/main/openapi/credentially-gateway-openapi-original.json
- filename: credentially-webhook-openapi-original.json
  format: json
  label: Credentially Webhook API
  slug: credentially-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credentially/refs/heads/main/openapi/credentially-webhook-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: credentially.io
  spf: true
hosts:
- cert_expires: Oct 15 04:12:36 2026 GMT
  host: credentially.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: app.credentially.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Credentially Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Credentially, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Credentially
provider_slug: credentially
slug: credentially-domain-security
source_filename: credentially-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: credentially.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 04:12:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.credentially.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: credentially.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credentially/refs/heads/main/security/credentially-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Healthcare
- Credentialing
- Compliance
- Onboarding
- Workforce
- Identity Verification
- Background Checks
- NHS
- Company
---
