---
api_specs:
- filename: breeze-openapi-original.json
  format: json
  label: Breeze API
  slug: breeze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/openapi/breeze-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: breeze.com
  spf: true
hosts:
- cert_expires: Sep 11 05:19:22 2026 GMT
  host: breeze.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 22 07:47:50 2026 GMT
  host: api.breeze.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Breeze Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Breeze, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Breeze
provider_slug: breeze
slug: breeze-domain-security
source_filename: breeze-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: breeze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 05:19:22 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.breeze.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 07:47:50 2026 GMT\n  hsts: null\ndomains:\n- domain: breeze.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breeze/refs/heads/main/security/breeze-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Solana
- Yield
- DeFi
- Payments
- Blockchain
- API
- AI Agents
---
