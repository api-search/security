---
api_specs:
- filename: ozow-openapi.yml
  format: yaml
  label: Ozow Payments API
  slug: ozow-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ozow/refs/heads/main/openapi/ozow-openapi.yml
- filename: ozow-openapi.yml
  format: yaml
  label: Ozow Transactions API
  slug: ozow-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ozow/refs/heads/main/openapi/ozow-openapi.yml
- filename: ozow-openapi.yml
  format: yaml
  label: Ozow Bank List API
  slug: ozow-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ozow/refs/heads/main/openapi/ozow-openapi.yml
- filename: ozow-openapi.yml
  format: yaml
  label: Ozow Refunds API
  slug: ozow-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ozow/refs/heads/main/openapi/ozow-openapi.yml
description: ''
domains:
- dmarc: true
  dmarc_pct: 100
  dmarc_policy: reject
  domain: ozow.com
  security_txt: false
  security_txt_note: https://ozow.com/.well-known/security.txt returned HTTP 404 at probe time.
  spf: true
  spf_record: v=spf1 redirect=_s7wa9pc2t.sdmarc.net
hosts:
- cert_expires: Sep 22 15:12:02 2026 GMT
  cert_issuer: Let's Encrypt (YR2)
  host: ozow.com
  hsts: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
- cert_expires: Jan 30 23:59:59 2027 GMT
  cert_issuer: Amazon (RSA 2048 M01)
  host: api.ozow.com
  hsts: null
  http_note: Root returns 404; API endpoints require a path plus query/body and ApiKey header.
  http_status: 404
  https: true
- cert_expires: Oct 11 01:03:21 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: hub.ozow.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 200
  https: true
- cert_expires: Sep  8 04:17:55 2026 GMT
  cert_issuer: Google Trust Services (WE1)
  host: dash.ozow.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  http_status: 302
  https: true
- cert_expires: Oct 16 23:59:59 2026 GMT
  cert_issuer: Amazon (RSA 2048 M01)
  host: pay.ozow.com
  http_note: Redirects into the hosted secure bank-selection flow (pay.ozow.com/:uuid/Secure).
  http_status: 302
  https: true
kind: domain-security
layout: security
method: probed
name: Ozow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ozow, probed live across 5 host(s) and 1 registrable domain(s). 5 host(s) serve HTTPS; 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ozow
provider_slug: ozow
slug: ozow-domain-security
source_filename: ozow-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ozow.com\n  https: true\n  http_status: 200\n  cert_expires: Sep 22 15:12:02 2026 GMT\n  cert_issuer: Let's Encrypt (YR2)\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.ozow.com\n  https: true\n  http_status: 404\n  http_note: Root returns 404; API endpoints require a path plus query/body and ApiKey header.\n  cert_expires: Jan 30 23:59:59 2027 GMT\n  cert_issuer: Amazon (RSA 2048 M01)\n  hsts: null\n- host: hub.ozow.com\n  https: true\n  http_status: 200\n  cert_expires: Oct 11 01:03:21 2026 GMT\n  cert_issuer: Google Trust Services (WE1)\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: dash.ozow.com\n  https: true\n  http_status: 302\n  cert_expires: Sep  8 04:17:55 2026 GMT\n  cert_issuer: Google Trust Services (WE1)\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: pay.ozow.com\n  https:\
  \ true\n  http_status: 302\n  http_note: Redirects into the hosted secure bank-selection flow (pay.ozow.com/:uuid/Secure).\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  cert_issuer: Amazon (RSA 2048 M01)\ndomains:\n- domain: ozow.com\n  spf: true\n  spf_record: v=spf1 redirect=_s7wa9pc2t.sdmarc.net\n  dmarc: true\n  dmarc_policy: reject\n  dmarc_pct: 100\n  security_txt: false\n  security_txt_note: https://ozow.com/.well-known/security.txt returned HTTP 404 at probe time.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ozow/refs/heads/main/security/ozow-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Payments
- Instant EFT
- Pay by Bank
- Fintech
- South Africa
---
