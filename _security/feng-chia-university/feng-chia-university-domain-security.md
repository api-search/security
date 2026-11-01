---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: gis.tw
  spf: true
hosts:
- cert_expires: Jan  3 16:28:09 2027 GMT
  host: www.gis.tw
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Feng Chia University Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Feng Chia University, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Feng Chia University
provider_slug: feng-chia-university
slug: feng-chia-university-domain-security
source_filename: feng-chia-university-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gis.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 16:28:09 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gis.tw\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/feng-chia-university/security/feng-chia-university-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- GIS
- Smart City
- AIoT
- Open Data
- Data Analysis
- GeoAI
---
