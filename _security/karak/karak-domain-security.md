---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: opengdp.network
  spf: false
hosts:
- cert_expires: Oct  5 19:23:47 2026 GMT
  host: opengdp.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Karak Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Karak, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Karak
provider_slug: karak
slug: karak-domain-security
source_filename: karak-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opengdp.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 19:23:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: opengdp.network\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/karak/refs/heads/main/security/karak-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto
- Blockchain
- Restaking
- Stablecoins
- Tokenization
- EVM
- Infrastructure
- DeFi
- Web3
---
