---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: injective.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: injective.network
  spf: true
hosts:
- cert_expires: Sep 19 13:26:17 2026 GMT
  host: injective.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 17:13:21 2026 GMT
  host: docs.injective.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 30 03:09:46 2026 GMT
  host: api.injective.network
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Injective Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Injective, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Injective
provider_slug: injective
slug: injective-domain-security
source_filename: injective-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: injective.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 13:26:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.injective.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 17:13:21 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.injective.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 03:09:46 2026 GMT\n  hsts: null\ndomains:\n- domain: injective.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: injective.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/injective/refs/heads/main/security/injective-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Blockchain
- DeFi
- Trading
- Derivatives
- Web3
- Layer 1
- Cosmos
- Tokenization
- Payments
- AI Agents
---
