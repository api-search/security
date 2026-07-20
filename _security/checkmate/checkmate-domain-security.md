---
api_specs:
- filename: checkmate-openstock-openapi-original.json
  format: json
  label: OpenStock API
  slug: openstock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/checkmate/refs/heads/main/openapi/checkmate-openstock-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: joincheckmate.com
  spf: true
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: openstock.sh
  spf: false
hosts:
- cert_expires: Oct  5 04:29:29 2026 GMT
  host: joincheckmate.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 20:20:54 2026 GMT
  host: openstock.sh
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 14 20:20:54 2026 GMT
  host: api.openstock.sh
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Checkmate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Checkmate, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Checkmate
provider_slug: checkmate
slug: checkmate-domain-security
source_filename: checkmate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: joincheckmate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 04:29:29 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: openstock.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:20:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.openstock.sh\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 20:20:54 2026 GMT\n  hsts: false\ndomains:\n- domain: joincheckmate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: openstock.sh\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/checkmate/refs/heads/main/security/checkmate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer
- Commerce
- Ecommerce
- Shopping
- Discount Codes
- Coupons
- Merchants
- MCP
- Agentic Commerce
- Retail
- API
---
