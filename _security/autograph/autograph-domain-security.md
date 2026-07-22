---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: autograph.io
  spf: true
hosts:
- cert_expires: Oct 18 23:59:59 2026 GMT
  host: autograph.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Autograph Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Autograph, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Autograph
provider_slug: autograph
slug: autograph-domain-security
source_filename: autograph-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: autograph.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 18 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: autograph.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/autograph/refs/heads/main/security/autograph-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fan Engagement
- Digital Collectibles
- NFT
- Web3
- Sports
- Entertainment
- Blockchain
- Consumer
---
