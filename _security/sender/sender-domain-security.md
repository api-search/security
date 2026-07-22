---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: senderwallet.io
  spf: true
hosts:
- cert_expires: Oct  3 02:41:31 2026 GMT
  host: senderwallet.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sender Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sender, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Sender
provider_slug: sender
slug: sender-domain-security
source_filename: sender-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: senderwallet.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 02:41:31 2026 GMT\n  hsts: false\ndomains:\n- domain: senderwallet.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sender/refs/heads/main/security/sender-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Crypto
- Wallet
- Web3
- Blockchain
- Ethereum
- NEAR
- DeFi
- Self-Custody
---
