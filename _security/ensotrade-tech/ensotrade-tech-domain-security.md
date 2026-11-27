---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ensotrade.tech
  spf: true
hosts:
- cert_expires: Feb  4 13:26:46 2027 GMT
  host: ensotrade.tech
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EnsoTrade Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EnsoTrade, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EnsoTrade
provider_slug: ensotrade-tech
slug: ensotrade-tech-domain-security
source_filename: ensotrade-tech-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ensotrade.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 13:26:46 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: ensotrade.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/ensotrade-tech/security/ensotrade-tech-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Finance
- Data
- Artificial Intelligence
- Trading
- Platform
---
