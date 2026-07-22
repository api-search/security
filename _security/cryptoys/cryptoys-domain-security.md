---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: digitoys.io
  spf: true
hosts:
- cert_expires: Sep 14 23:59:59 2026 GMT
  host: digitoys.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cryptoys Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cryptoys, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cryptoys
provider_slug: cryptoys
slug: cryptoys-domain-security
source_filename: cryptoys-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: digitoys.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 14 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: digitoys.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cryptoys/refs/heads/main/security/cryptoys-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web3
- NFT
- Digital Collectibles
- Blockchain
- Gaming
- Toys
- Consumer
---
