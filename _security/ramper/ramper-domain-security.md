---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ramper.xyz
  spf: true
hosts:
- cert_expires: Sep  6 08:50:14 2026 GMT
  host: ramper.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ramper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ramper, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Ramper
provider_slug: ramper
slug: ramper-domain-security
source_filename: ramper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ramper.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 08:50:14 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ramper.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ramper/refs/heads/main/security/ramper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web3
- Wallet
- Embedded Wallet
- Blockchain
- Social Login
- Authentication
- SDK
- NFT
- Cryptocurrency
- DeFi
---
