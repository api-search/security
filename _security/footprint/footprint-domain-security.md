---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Footprint Analytics Data API
  slug: footprint-analytics-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: footprint.network
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: readme.io
  spf: true
hosts:
- cert_expires: Aug 12 13:48:28 2026 GMT
  host: www.footprint.network
  hsts: true
  hsts_max_age: 15724800
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 23:59:59 2026 GMT
  host: api.footprint.network
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:12:37 2026 GMT
  host: fp-api.readme.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Footprint Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Footprint Analytics, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Footprint Analytics
provider_slug: footprint
slug: footprint-domain-security
source_filename: footprint-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.footprint.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 13:48:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15724800\n- host: api.footprint.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 23:59:59 2026 GMT\n  hsts: null\n- host: fp-api.readme.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:12:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: footprint.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: readme.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/footprint/refs/heads/main/security/footprint-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- DeFi
- NFT
- GameFi
- Token Analytics
- On-Chain Data
- Web3
- Crypto
---
