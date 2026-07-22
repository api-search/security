---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: coin98.com
  spf: true
hosts:
- cert_expires: Sep 24 15:33:20 2026 GMT
  host: coin98.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Coin98 Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Coin98, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Coin98
provider_slug: coin98
slug: coin98-domain-security
source_filename: coin98-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: coin98.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 15:33:20 2026 GMT\n  hsts: false\ndomains:\n- domain: coin98.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coin98/refs/heads/main/security/coin98-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto Web3
- Cryptocurrency Wallet
- DeFi
- Blockchain
- Web3
- Wallet SDK
- Developer Tools
---
