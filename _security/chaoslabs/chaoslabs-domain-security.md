---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: chaoslabs.xyz
  spf: true
hosts:
- cert_expires: Aug 21 12:02:50 2026 GMT
  host: chaoslabs.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Chaoslabs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Chaoslabs, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Chaoslabs
provider_slug: chaoslabs
slug: chaoslabs-domain-security
source_filename: chaoslabs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: chaoslabs.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 12:02:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: chaoslabs.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chaoslabs/refs/heads/main/security/chaoslabs-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Oracles
- Risk Management
- DeFi
- Blockchain
- Onchain Data
- Economic Security
- Price Feeds
- Crypto
- AI
---
