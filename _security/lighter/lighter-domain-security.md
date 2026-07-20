---
api_specs:
- filename: lighter-zklighter-openapi-original.json
  format: json
  label: zkLighter API
  slug: zklighter
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/openapi/lighter-zklighter-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lighter.xyz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: elliot.ai
  spf: true
hosts:
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: lighter.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 21 18:12:40 2026 GMT
  host: apidocs.lighter.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: mainnet.zklighter.elliot.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lighter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lighter, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lighter
provider_slug: lighter
slug: lighter-domain-security
source_filename: lighter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lighter.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.lighter.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:12:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: mainnet.zklighter.elliot.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: lighter.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: elliot.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lighter/refs/heads/main/security/lighter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trading
- Cryptocurrency
- Decentralized Finance
- Perpetual Futures
- Exchange
- Blockchain
- Zero Knowledge
- Market Data
- WebSockets
---
