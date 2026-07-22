---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tiplink.io
  spf: true
hosts:
- cert_expires: Sep 17 21:02:26 2026 GMT
  host: tiplink.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tiplink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TipLink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: TipLink
provider_slug: tiplink
slug: tiplink-domain-security
source_filename: tiplink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tiplink.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 21:02:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tiplink.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tiplink/refs/heads/main/security/tiplink-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Web3
- Solana
- Wallet
- SDK
- Payments
- Web3
---
