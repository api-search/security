---
api_specs:
- filename: ostium-labs-prices-asyncapi.yml
  format: yaml
  label: Ostium Builder API
  slug: ostium-builder-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostium-labs/refs/heads/main/asyncapi/ostium-labs-prices-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ostium.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ostium.io
  spf: true
hosts:
- cert_expires: Sep 17 05:22:59 2026 GMT
  host: www.ostium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 23:40:48 2026 GMT
  host: docs.ostium.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: builder.ostium.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ostium Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ostium Labs, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ostium Labs
provider_slug: ostium-labs
slug: ostium-labs-domain-security
source_filename: ostium-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ostium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 05:22:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.ostium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 23:40:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: builder.ostium.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ostium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ostium.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ostium-labs/refs/heads/main/security/ostium-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Perpetual Futures
- Decentralized Finance
- DeFi
- Trading
- Real World Assets
- Derivatives
- Arbitrum
- Blockchain
- Web3
- Market Data
- SDK
---
