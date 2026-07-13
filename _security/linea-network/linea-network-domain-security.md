---
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
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
name: Linea Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linea, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Linea
provider_slug: linea-network
slug: linea-network-domain-security
source_filename: linea-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linea.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 11:25:30 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: docs.linea.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 23:04:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: rpc.linea.build\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:39:22 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: linea.build\n  dnssec: true\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linea-network/refs/heads/main/security/linea-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Layer 2
- Ethereum
- zkEVM
- EVM Equivalence
- JSON-RPC
- Consensys
---
