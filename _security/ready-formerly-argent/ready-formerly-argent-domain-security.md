---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ready.co
  spf: true
hosts:
- cert_expires: Sep  5 19:54:56 2026 GMT
  host: www.ready.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ready Formerly Argent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ready (formerly Argent), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Ready (formerly Argent)
provider_slug: ready-formerly-argent
slug: ready-formerly-argent-domain-security
source_filename: ready-formerly-argent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ready.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 19:54:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ready.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ready-formerly-argent/refs/heads/main/security/ready-formerly-argent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Fintech
- Cryptocurrency
- Wallet
- Blockchain
- Starknet
- Ethereum
- SDK
- Web3
- Account Abstraction
---
