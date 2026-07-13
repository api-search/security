---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: envio.dev
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: hypersync.xyz
  spf: false
hosts:
- cert_expires: Oct  6 07:37:27 2026 GMT
  host: envio.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 22:22:50 2026 GMT
  host: docs.envio.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 09:29:19 2026 GMT
  host: eth.hypersync.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Envio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Envio, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Envio
provider_slug: envio
slug: envio-domain-security
source_filename: envio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: envio.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 07:37:27 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.envio.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 22:22:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: eth.hypersync.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 09:29:19 2026 GMT\n  hsts: null\ndomains:\n- domain: envio.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hypersync.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envio/refs/heads/main/security/envio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Indexer
- GraphQL
- Web3
- EVM
- Smart Contracts
- Data
- HyperSync
- HyperIndex
- Multichain
---
