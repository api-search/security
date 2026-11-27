---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: fmcg.network
  spf: true
hosts:
- cert_expires: Jan 18 16:02:49 2027 GMT
  host: fmcg.network
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: fmcg.network Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for fmcg.network, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: fmcg.network
provider_slug: fmcg-network
slug: fmcg-network-domain-security
source_filename: fmcg-network-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fmcg.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 16:02:49 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fmcg.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/fmcg-network/security/fmcg-network-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Consumer Packaged Goods
- FoodCompliance
- Artificial Intelligence
- Data Integration
---
