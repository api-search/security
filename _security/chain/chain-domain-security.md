---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: chain.com
  spf: true
hosts:
- cert_expires: Sep 12 07:57:15 2026 GMT
  host: chain.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 07:39:19 2026 GMT
  host: api.chain.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chain, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Chain
provider_slug: chain
slug: chain-domain-security
source_filename: chain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 07:57:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.chain.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 07:39:19 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: chain.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chain/refs/heads/main/security/chain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Stablecoin
- Cryptocurrency
- Blockchain
- Financial Services
- Wallets
- Cards
- Cross-Border Payments
- API
---
