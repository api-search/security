---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: grapes.network
  spf: false
hosts:
- cert_expires: Sep 13 21:16:32 2026 GMT
  host: grapes.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Grapes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grapes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Grapes
provider_slug: grapes
slug: grapes-domain-security
source_filename: grapes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grapes.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 21:16:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grapes.network\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grapes/refs/heads/main/security/grapes-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Crypto Web3
- Solana
- DAO
- Reputation
- Governance
- Access Control
- Web3 Infrastructure
---
