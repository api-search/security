---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: orabandamining.com.au
  spf: true
hosts:
- cert_expires: Dec 16 19:40:53 2026 GMT
  host: orabandamining.com.au
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ora Banda Mining Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ora Banda Mining, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Ora Banda Mining
provider_slug: ora-banda-mining
slug: ora-banda-mining-domain-security
source_filename: ora-banda-mining-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orabandamining.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 16 19:40:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: orabandamining.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ora-banda-mining/refs/heads/main/security/ora-banda-mining-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Mining
- Gold
- Gold Production
- Mineral Exploration
- Western Australia
- Australia
---
