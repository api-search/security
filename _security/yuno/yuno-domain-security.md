---
api_specs:
- filename: yuno-openapi-original.json
  format: json
  label: Yuno Payments API
  slug: yuno-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yuno/refs/heads/main/openapi/yuno-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: y.uno
  spf: true
hosts:
- cert_expires: Sep 28 13:54:57 2026 GMT
  host: y.uno
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 15:50:54 2026 GMT
  host: docs.y.uno
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 13 23:59:59 2027 GMT
  host: api.y.uno
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yuno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yuno, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yuno
provider_slug: yuno
slug: yuno-domain-security
source_filename: yuno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: y.uno\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 13:54:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.y.uno\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 15:50:54 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.y.uno\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 13 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: y.uno\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yuno/refs/heads/main/security/yuno-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Payment Orchestration
- Fintech
- Checkout
- Payouts
- Subscriptions
- API
---
