---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rain.xyz
  spf: true
hosts:
- cert_expires: Oct  5 23:44:31 2026 GMT
  host: www.rain.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rain
provider_slug: rain
slug: rain-domain-security
source_filename: rain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rain.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 23:44:31 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: rain.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rain/refs/heads/main/security/rain-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Stablecoins
- Payments
- Card Issuing
- Fintech
- Cross-Border Payments
- Crypto
- Wallets
- Money Movement
- API
---
