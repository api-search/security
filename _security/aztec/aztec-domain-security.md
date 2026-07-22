---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: aztec.network
  spf: true
hosts:
- cert_expires: Sep 27 09:28:51 2026 GMT
  host: aztec.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aztec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aztec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Aztec
provider_slug: aztec
slug: aztec-domain-security
source_filename: aztec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aztec.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 09:28:51 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aztec.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aztec/refs/heads/main/security/aztec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- Privacy
- Zero-Knowledge
- Ethereum
- Layer 2
- Smart Contracts
- Cryptography
- Developer Tools
- Web3
---
