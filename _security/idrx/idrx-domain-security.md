---
api_specs:
- filename: idrx-openapi.yml
  format: yaml
  label: IDRX API
  slug: idrx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/idrx/refs/heads/main/openapi/idrx-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: idrx.co
  spf: true
hosts:
- cert_expires: Sep  6 16:05:27 2026 GMT
  host: idrx.co
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Idrx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IDRX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: IDRX
provider_slug: idrx
slug: idrx-domain-security
source_filename: idrx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: idrx.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 16:05:27 2026 GMT\n  hsts: false\ndomains:\n- domain: idrx.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idrx/refs/heads/main/security/idrx-domain-security.yml
summary_line: TLSv1.3
tags:
- Stablecoin
- Cryptocurrency
- Payments
- Blockchain
- Fintech
- Indonesia
- Rupiah
- Web3
- On-Ramp
- Digital Currency
---
