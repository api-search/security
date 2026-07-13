---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: quant.network
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: overledger.dev
  spf: false
hosts:
- cert_expires: Sep 12 03:14:43 2026 GMT
  host: www.quant.network
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 11:33:18 2026 GMT
  host: docs.overledger.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Quant Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Quant Network, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Quant Network
provider_slug: quant
slug: quant-domain-security
source_filename: quant-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.quant.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 03:14:43 2026 GMT\n  hsts: false\n- host: docs.overledger.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 11:33:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: quant.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: overledger.dev\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quant/refs/heads/main/security/quant-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- Distributed Ledger
- Interoperability
- Overledger
- Smart Contracts
- Digital Assets
- Web3
---
