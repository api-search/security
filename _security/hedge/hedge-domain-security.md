---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: hedge.so
  spf: true
hosts:
- cert_expires: Aug 25 15:15:41 2026 GMT
  host: www.hedge.so
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hedge Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hedge, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Hedge
provider_slug: hedge
slug: hedge-domain-security
source_filename: hedge-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hedge.so\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 15:15:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hedge.so\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hedge/refs/heads/main/security/hedge-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Crypto
- DeFi
- Solana
- Stablecoin
- Lending
- Blockchain
---
