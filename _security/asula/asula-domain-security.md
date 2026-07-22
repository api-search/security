---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: asula.xyz
  spf: true
hosts:
- cert_expires: Aug 26 23:25:01 2026 GMT
  host: asula.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Asula Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Asula, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Asula
provider_slug: asula
slug: asula-domain-security
source_filename: asula-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: asula.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 23:25:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: asula.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/asula/refs/heads/main/security/asula-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto
- Bitcoin
- Blockchain
- Finance
- Fintech
- Lending
- Wallet
---
