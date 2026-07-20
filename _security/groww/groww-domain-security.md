---
api_specs:
- filename: groww-trade-api-openapi.yml
  format: yaml
  label: Groww Trading API
  slug: groww-trade-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/openapi/groww-trade-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: groww.in
  spf: true
hosts:
- cert_expires: Oct  7 10:48:30 2026 GMT
  host: groww.in
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  7 10:48:30 2026 GMT
  host: api.groww.in
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Groww Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Groww, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Groww
provider_slug: groww
slug: groww-domain-security
source_filename: groww-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: groww.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:48:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.groww.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:48:30 2026 GMT\n  hsts: null\ndomains:\n- domain: groww.in\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groww/refs/heads/main/security/groww-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Fintech
- Trading
- Investing
- Stock Broking
- Market Data
- Algorithmic Trading
- India
---
