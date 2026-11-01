---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: grapes.network
  spf: false
hosts:
- cert_expires: Jan  9 22:28:20 2027 GMT
  host: grapes.network
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Grapes Network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Grapes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Grapes
provider_slug: grapes-network
slug: grapes-network-domain-security
source_filename: grapes-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: grapes.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  9 22:28:20 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: grapes.network\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/grapes-network/security/grapes-network-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Identity
- Reputation
- Access Control
- Governance
- DAO Infrastructure
- Discord Bots
- Solana
---
