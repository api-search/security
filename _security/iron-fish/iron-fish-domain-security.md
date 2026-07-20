---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ironfish.network
  spf: true
hosts:
- cert_expires: Aug 19 19:09:43 2026 GMT
  host: ironfish.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Iron Fish Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Iron Fish, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Iron Fish
provider_slug: iron-fish
slug: iron-fish-domain-security
source_filename: iron-fish-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ironfish.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 19:09:43 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ironfish.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iron-fish/refs/heads/main/security/iron-fish-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Blockchain
- Cryptocurrency
- Privacy
- Zero Knowledge
- Layer 1
- Web3
- RPC
- Wallet
---
