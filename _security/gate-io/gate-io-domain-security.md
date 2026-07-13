---
api_specs:
- filename: swagger.json
  format: json
  label: Gate API v4 — Spot & Margin
  slug: gate-api-v4-spot-margin
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/gateio/rest-v4/master/swagger.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: gate.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: gate.com
  spf: true
hosts:
- cert_expires: Oct  4 01:13:54 2026 GMT
  host: www.gate.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 00:48:20 2026 GMT
  host: www.gate.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 27 23:59:59 2026 GMT
  host: api.gateio.ws
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gate Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gate.io, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Gate.io
provider_slug: gate-io
slug: gate-io-domain-security
source_filename: gate-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gate.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:13:54 2026 GMT\n  hsts: null\n- host: www.gate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 00:48:20 2026 GMT\n  hsts: null\n- host: api.gateio.ws\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 27 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gate.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: gate.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gate-io/refs/heads/main/security/gate-io-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cryptocurrency
- Exchange
- Trading
- Spot Trading
- Margin Trading
- Futures
- Options
- WebSocket
- Market Data
- Wallet
---
