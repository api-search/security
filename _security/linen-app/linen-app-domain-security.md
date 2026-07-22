---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: linen.app
  spf: true
hosts:
- cert_expires: Oct  4 20:41:09 2026 GMT
  host: linen.app
  hsts: true
  hsts_max_age: 631138519
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Linen App Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Linen App, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Linen App
provider_slug: linen-app
slug: linen-app-domain-security
source_filename: linen-app-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: linen.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 20:41:09 2026 GMT\n  hsts: true\n  hsts_max_age: 631138519\ndomains:\n- domain: linen.app\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/linen-app/refs/heads/main/security/linen-app-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Wallet
- Cryptocurrency
- Ethereum
- DeFi
- Self Custody
- Multisig
- Blockchain
- Discontinued
---
