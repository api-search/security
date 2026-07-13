---
api_specs:
- filename: lbank-spot-market-rest-api.json
  format: json
  label: LBank Spot Market REST API
  slug: spot-market-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/openapi/lbank-spot-market-rest-api.json
- filename: lbank-spot-trading-rest-api.json
  format: json
  label: LBank Spot Trading REST API
  slug: spot-trading-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/openapi/lbank-spot-trading-rest-api.json
- filename: lbank-wallet-rest-api.json
  format: json
  label: LBank Wallet REST API
  slug: wallet-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/openapi/lbank-wallet-rest-api.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: lbank.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: lbkex.com
  spf: false
hosts:
- cert_expires: Sep 30 12:19:41 2026 GMT
  host: www.lbank.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 21:48:50 2026 GMT
  host: api.lbkex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 20 06:11:13 2027 GMT
  host: www.lbkex.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Lbank Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LBank, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: LBank
provider_slug: lbank
slug: lbank-domain-security
source_filename: lbank-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lbank.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 12:19:41 2026 GMT\n  hsts: false\n- host: api.lbkex.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 21 21:48:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.lbkex.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb 20 06:11:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lbank.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: lbkex.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lbank/refs/heads/main/security/lbank-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Cryptocurrency
- Exchange
- Trading
- Market Data
- Finance
- Blockchain
---
