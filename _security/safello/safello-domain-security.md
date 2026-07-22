---
api_specs:
- filename: safello-institutional-openapi.json
  format: json
  label: Safello Institutional API
  slug: safello-institutional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/openapi/safello-institutional-openapi.json
- filename: safello-app-openapi.json
  format: json
  label: Safello App API
  slug: safello-app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/openapi/safello-app-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: safello.com
  spf: true
hosts:
- cert_expires: Aug 22 13:07:12 2026 GMT
  host: safello.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 11 23:59:59 2026 GMT
  host: app.safello.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 16 23:59:59 2027 GMT
  host: api.safello.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Safello Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Safello, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Safello
provider_slug: safello
slug: safello-domain-security
source_filename: safello-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: safello.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 13:07:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.safello.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 11 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.safello.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 16 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: safello.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/safello/refs/heads/main/security/safello-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Cryptocurrency
- Bitcoin
- Brokerage
- Payments
- Sweden
- Trading
- KYC
- BankID
---
