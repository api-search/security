---
api_specs:
- filename: payabli-api-reference-openapi.json
  format: json
  label: Payabli API
  slug: payabli-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/payabli/refs/heads/main/openapi/payabli-api-reference-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: payabli.com
  spf: true
hosts:
- cert_expires: Sep 16 00:02:18 2026 GMT
  host: payabli.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 08:37:42 2026 GMT
  host: docs.payabli.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 23:59:59 2026 GMT
  host: api.payabli.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Payabli Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Payabli, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Payabli
provider_slug: payabli
slug: payabli-domain-security
source_filename: payabli-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: payabli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 00:02:18 2026 GMT\n  hsts: false\n- host: docs.payabli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:37:42 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.payabli.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: payabli.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/payabli/refs/heads/main/security/payabli-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Embedded Payments
- Fintech
- Payment Processing
- Payments API
- Payouts
- Billing
- ACH
- Cards
- Tokenization
- Webhooks
---
