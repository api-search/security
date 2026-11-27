---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: callejear.fr
  spf: true
hosts:
- cert_expires: Jan 29 22:18:32 2027 GMT
  host: callejear.fr
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Callejear.fr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Callejear.fr, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Callejear.fr
provider_slug: callejear-fr
slug: callejear-fr-domain-security
source_filename: callejear-fr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: callejear.fr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 29 22:18:32 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: callejear.fr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/callejear-fr/security/callejear-fr-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Open Data
- Real Estate
- Geospatial
- Addresses
- France
- Quality Of Life
- MCP
---
