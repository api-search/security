---
api_specs:
- filename: derivadex-exchange-openapi.yml
  format: yaml
  label: DerivaDEX Exchange & Stats API
  slug: derivadex-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/derivadex/refs/heads/main/openapi/derivadex-exchange-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: derivadex.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: derivadex.io
  spf: true
hosts:
- cert_expires: Aug 31 16:17:38 2026 GMT
  host: derivadex.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 07:55:42 2026 GMT
  host: docs.derivadex.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 31 16:17:38 2026 GMT
  host: exchange.derivadex.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Derivadex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DerivaDEX, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: DerivaDEX
provider_slug: derivadex
slug: derivadex-domain-security
source_filename: derivadex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: derivadex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:17:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.derivadex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 07:55:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: exchange.derivadex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 16:17:38 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: derivadex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: derivadex.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/derivadex/refs/heads/main/security/derivadex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Defi Derivatives
- Cryptocurrency
- Derivatives
- Perpetual Swaps
- Decentralized Exchange
- Trading
- Blockchain
- Market Data
- DeFi
---
