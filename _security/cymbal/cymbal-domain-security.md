---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cymbal.xyz
  spf: false
hosts:
- cert_expires: Oct  4 05:45:41 2026 GMT
  host: cymbal.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cymbal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cymbal, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Cymbal
provider_slug: cymbal
slug: cymbal-domain-security
source_filename: cymbal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cymbal.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 05:45:41 2026 GMT\n  hsts: null\ndomains:\n- domain: cymbal.xyz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cymbal/refs/heads/main/security/cymbal-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Consumer
- Blockchain
- Ethereum
- Block Explorer
- Web3
- Crypto Data
- Acquired
---
