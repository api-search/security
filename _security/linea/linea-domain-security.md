---
api_specs:
- filename: linea-token-api-openapi.json
  format: json
  label: Linea Token API
  slug: token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/linea/refs/heads/main/openapi/linea-token-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: linea.build
  spf: true
hosts:
- cert_expires: Sep  4 11:25:30 2026 GMT
  host: linea.build
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 23:04:57 2026 GMT
  host: docs.linea.build
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 12:39:22 2026 GMT
  host: rpc.linea.build
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linea Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linea, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Linea
provider_slug: linea
slug: linea-domain-security
source_filename: linea-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linea.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 11:25:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.linea.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:04:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rpc.linea.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:39:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: linea.build\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linea/refs/heads/main/security/linea-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Ethereum
- Layer 2
- ZK-EVM
- Web3
- DeFi
- Smart Contracts
- JSON-RPC
- Tokens
- ConsenSys
---
