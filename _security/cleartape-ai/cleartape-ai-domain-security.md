---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cleartape.ai
  spf: true
hosts:
- cert_expires: Jan  8 22:19:56 2027 GMT
  host: cleartape.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cleartape Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Clear Tape, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Clear Tape
provider_slug: cleartape-ai
slug: cleartape-ai-domain-security
source_filename: cleartape-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cleartape.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 22:19:56 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cleartape.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/cleartape-ai/security/cleartape-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Finance
- Stock Screener
- Data
- Backtesting
- Free Tier
---
