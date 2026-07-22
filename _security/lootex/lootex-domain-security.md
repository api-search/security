---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lootex.io
  spf: true
hosts:
- cert_expires: Aug 29 11:15:34 2026 GMT
  host: lootex.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lootex Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lootex, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lootex
provider_slug: lootex
slug: lootex-domain-security
source_filename: lootex-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lootex.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 29 11:15:34 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: lootex.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lootex/refs/heads/main/security/lootex-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- NFT
- Marketplace
- Web3
- Blockchain
- Digital Assets
- Minting
---
