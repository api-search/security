---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: yieldguild.io
  spf: true
hosts:
- cert_expires: Aug 22 06:28:19 2026 GMT
  host: www.yieldguild.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Yield Guide Games Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Yield Guild Games, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Yield Guild Games
provider_slug: yield-guide-games
slug: yield-guide-games-domain-security
source_filename: yield-guide-games-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.yieldguild.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:28:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: yieldguild.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yield-guide-games/refs/heads/main/security/yield-guide-games-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Gaming
- Web3
- Blockchain
- DAO
- NFT
- Play-to-Earn
- Crypto
---
