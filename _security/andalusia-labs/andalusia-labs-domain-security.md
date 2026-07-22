---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: andalusia-labs.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: opengdp.network
  spf: false
hosts:
- cert_expires: Oct  5 20:13:50 2026 GMT
  host: andalusia-labs.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 19:23:47 2026 GMT
  host: opengdp.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Andalusia Labs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Andalusia Labs, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Andalusia Labs
provider_slug: andalusia-labs
slug: andalusia-labs-domain-security
source_filename: andalusia-labs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: andalusia-labs.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:13:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: opengdp.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:23:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: andalusia-labs.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: opengdp.network\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/andalusia-labs/refs/heads/main/security/andalusia-labs-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto
- Blockchain
- Stablecoins
- Tokenization
- Payments
- DeFi
- Infrastructure
- EVM
---
