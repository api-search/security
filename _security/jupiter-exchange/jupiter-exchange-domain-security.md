---
api_specs:
- filename: jupiter-exchange-openapi.yml
  format: yaml
  label: Jupiter Swap API
  slug: swap-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jupiter-exchange/refs/heads/main/openapi/jupiter-exchange-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: jup.ag
  spf: true
hosts:
- cert_expires: Oct  8 08:47:09 2026 GMT
  host: jup.ag
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: developers.jup.ag
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 23:59:59 2026 GMT
  host: lite-api.jup.ag
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jupiter Exchange Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jupiter, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Jupiter
provider_slug: jupiter-exchange
slug: jupiter-exchange-domain-security
source_filename: jupiter-exchange-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: jup.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 08:47:09 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developers.jup.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\n- host: lite-api.jup.ag\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: jup.ag\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jupiter-exchange/refs/heads/main/security/jupiter-exchange-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Solana
- DEX
- Aggregator
- Swap
- Limit Orders
- DCA
- Perpetuals
---
