---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: buienradar.nl
  spf: false
hosts:
- cert_expires: Jan 29 23:59:59 2027 GMT
  host: buienradar.nl
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Buienradar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Buienradar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Buienradar
provider_slug: buienradar
slug: buienradar-domain-security
source_filename: buienradar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: buienradar.nl\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15768000\ndomains:\n- domain: buienradar.nl\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/buienradar/security/buienradar-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Weather
- Radar
- Forecast
- Data
---
