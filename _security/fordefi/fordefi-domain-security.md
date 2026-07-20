---
api_specs:
- filename: fordefi-openapi-original.json
  format: json
  label: Fordefi API
  slug: fordefi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/openapi/fordefi-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: fordefi.com
  spf: true
hosts:
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: fordefi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 10 23:59:59 2026 GMT
  host: api.fordefi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fordefi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fordefi, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Fordefi
provider_slug: fordefi
slug: fordefi-domain-security
source_filename: fordefi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fordefi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fordefi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: fordefi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fordefi/refs/heads/main/security/fordefi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Security
- Cryptocurrency
- Digital Assets
- Wallet
- Custody
- Blockchain
- DeFi
- MPC
- Payments
---
