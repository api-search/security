---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: summonersarena.io
  spf: false
hosts:
- cert_expires: Oct 17 18:14:22 2026 GMT
  host: summonersarena.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Summoners Arena Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Summoners Arena, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Summoners Arena
provider_slug: summoners-arena
slug: summoners-arena-domain-security
source_filename: summoners-arena-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: summonersarena.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 17 18:14:22 2026 GMT\n  hsts: false\ndomains:\n- domain: summonersarena.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/summoners-arena/refs/heads/main/security/summoners-arena-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Crypto
- Gaming
- Web3
- NFT
- Blockchain
- Play-to-Earn
---
