---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amptoken.org
  spf: true
hosts:
- cert_expires: Sep 19 23:39:02 2026 GMT
  host: amptoken.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amp, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Amp
provider_slug: amp
slug: amp-domain-security
source_filename: amp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: amptoken.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 23:39:02 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: amptoken.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amp/refs/heads/main/security/amp-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto
- Blockchain
- Ethereum
- Collateral Token
- Payments
- DeFi
- Smart Contracts
- Tokenization
---
