---
api_specs:
- filename: rho-protocol-openapi-original.json
  format: json
  label: Rho Exchange API
  slug: rho-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rho-protocol/refs/heads/main/openapi/rho-protocol-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rho.trading
  spf: true
hosts:
- cert_expires: Oct 16 11:44:27 2026 GMT
  host: x.rho.trading
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 20 01:03:29 2026 GMT
  host: docs.rho.trading
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rho Protocol Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rho Protocol, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rho Protocol
provider_slug: rho-protocol
slug: rho-protocol-domain-security
source_filename: rho-protocol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: x.rho.trading\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 11:44:27 2026 GMT\n  hsts: null\n- host: docs.rho.trading\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 20 01:03:29 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rho.trading\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rho-protocol/refs/heads/main/security/rho-protocol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Trading
- DeFi
- Derivatives
- Capital Markets
- Blockchain
- Market Data
- WebSocket
- MCP
---
