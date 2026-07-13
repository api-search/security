---
api_specs:
- filename: openapi.json
  format: json
  label: Bitstamp REST API
  slug: bitstamp-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bitstamp/refs/heads/main/openapi/openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: bitstamp.net
  spf: true
hosts:
- cert_expires: Nov  7 23:59:59 2026 GMT
  host: www.bitstamp.net
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: ws.bitstamp.net
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Bitstamp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitstamp, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Bitstamp
provider_slug: bitstamp
slug: bitstamp-domain-security
source_filename: bitstamp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bitstamp.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 23:59:59 2026 GMT\n  hsts: false\n- host: ws.bitstamp.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: bitstamp.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitstamp/refs/heads/main/security/bitstamp-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cryptocurrency
- Exchange
- Trading
- Bitcoin
- Ethereum
- Spot Trading
- WebSocket
- Market Data
- Order Management
- Finance
---
