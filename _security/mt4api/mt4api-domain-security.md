---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mt4api.dev
  spf: true
hosts:
- cert_expires: Jan 17 21:14:26 2027 GMT
  host: mt4api.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mt4Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Noble Minds Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Noble Minds Media
provider_slug: mt4api
slug: mt4api-domain-security
source_filename: mt4api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mt4api.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 21:14:26 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mt4api.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mt4api/security/mt4api-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Finance
- Trading
- API
- MetaTrader
- Data
---
