---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: statistik.at
  spf: true
hosts:
- cert_expires: Apr 22 11:36:55 2027 GMT
  host: www.statistik.at
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Statistik Austria Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Statistik Austria, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Statistik Austria
provider_slug: statistik-at
slug: statistik-at-domain-security
source_filename: statistik-at-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.statistik.at\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr 22 11:36:55 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: statistik.at\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/statistik-at/security/statistik-at-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Official Statistics
- Government
- Open Data
- Austria
- Statistics
- Geospatial
- OGC
---
