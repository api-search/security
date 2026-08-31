---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: 3jane.xyz
  spf: true
hosts:
- cert_expires: Sep 18 04:46:24 2026 GMT
  host: www.3jane.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: 3Jane Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for 3Jane, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: 3Jane
provider_slug: 3jane
slug: 3jane-domain-security
source_filename: 3jane-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.3jane.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 04:46:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: 3jane.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/3jane/refs/heads/main/security/3jane-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto Defi
- DeFi
- Lending
- Credit
- Uncollateralized Lending
- Stablecoin
- Money Market
- Ethereum
- Yield
---
