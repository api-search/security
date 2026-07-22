---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: candy.io
  spf: true
hosts:
- cert_expires: Aug 26 18:35:55 2026 GMT
  host: www.candy.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Candy Fanatics Fka Candy Digital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Candy Fanatics (fka Candy Digital), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Candy Fanatics (fka Candy Digital)
provider_slug: candy-fanatics-fka-candy-digital
slug: candy-fanatics-fka-candy-digital-domain-security
source_filename: candy-fanatics-fka-candy-digital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.candy.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 18:35:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: candy.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/candy-fanatics-fka-candy-digital/refs/heads/main/security/candy-fanatics-fka-candy-digital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Web3
- Digital Collectibles
- NFT
- MLB
- Sports
- Trading Cards
- Consumer
---
