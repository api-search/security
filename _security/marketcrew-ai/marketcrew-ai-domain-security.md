---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marketcrew.ai
  spf: false
hosts:
- cert_expires: Jan 31 00:17:49 2027 GMT
  host: marketcrew.ai
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MarketCrew Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MarketCrew, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: MarketCrew
provider_slug: marketcrew-ai
slug: marketcrew-ai-domain-security
source_filename: marketcrew-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marketcrew.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 00:17:49 2027 GMT\n  hsts: null\ndomains:\n- domain: marketcrew.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/marketcrew-ai/security/marketcrew-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Finance
- Market Data
- Trading
---
