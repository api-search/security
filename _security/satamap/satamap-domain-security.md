---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: satamap.com.au
  spf: false
hosts:
- cert_expires: Jan  4 22:27:50 2027 GMT
  host: satamap.com.au
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Satamap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Satamap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Satamap
provider_slug: satamap
slug: satamap-domain-security
source_filename: satamap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: satamap.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 22:27:50 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: satamap.com.au\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/satamap/security/satamap-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Satellite
- Imagery
- Agriculture
- Remote Sensing
- SaaS
---
