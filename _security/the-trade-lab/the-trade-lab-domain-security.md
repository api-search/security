---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: thetradelab.ai
  spf: false
hosts:
- cert_expires: Jan 15 17:05:48 2027 GMT
  host: thetradelab.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: The Trade Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for The Trade Lab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: The Trade Lab
provider_slug: the-trade-lab
slug: the-trade-lab-domain-security
source_filename: the-trade-lab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: thetradelab.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 17:05:48 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: thetradelab.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/the-trade-lab/security/the-trade-lab-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- TradeCompliance
- InternationalTrade
- SaaS
---
