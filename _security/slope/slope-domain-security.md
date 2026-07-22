---
api_specs:
- filename: slope-v4-openapi.json
  format: json
  label: Slope v4 API
  slug: slope-v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/openapi/slope-v4-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: slopepay.com
  spf: true
hosts:
- cert_expires: Oct  1 12:58:48 2026 GMT
  host: www.slopepay.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 23:59:59 2026 GMT
  host: api.slopepay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: api.sandbox.slopepay.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Slope Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Slope, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Slope
provider_slug: slope
slug: slope-domain-security
source_filename: slope-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.slopepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 12:58:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.slopepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 23:59:59 2026 GMT\n  hsts: null\n- host: api.sandbox.slopepay.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: slopepay.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/slope/refs/heads/main/security/slope-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Payments
- Embedded Finance
- BNPL
- Lending
- Credit
- B2B
- Checkout
---
