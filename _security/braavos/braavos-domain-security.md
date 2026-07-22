---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: braavos.app
  spf: false
hosts:
- cert_expires: Jan 15 23:59:59 2027 GMT
  host: braavos.app
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Braavos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Braavos, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Braavos
provider_slug: braavos
slug: braavos-domain-security
source_filename: braavos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: braavos.app\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: braavos.app\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/braavos/refs/heads/main/security/braavos-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Crypto
- Wallet
- Blockchain
- Starknet
- Bitcoin
- Self-Custody
- Account Abstraction
- Web3
---
