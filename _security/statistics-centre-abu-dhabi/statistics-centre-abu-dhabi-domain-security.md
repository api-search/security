---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scad.ae
  spf: true
hosts:
- cert_expires: Dec  6 08:49:06 2026 GMT
  host: www.scad.ae
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Statistics Centre Abu Dhabi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Statistics Centre - Abu Dhabi, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Statistics Centre - Abu Dhabi
provider_slug: statistics-centre-abu-dhabi
slug: statistics-centre-abu-dhabi-domain-security
source_filename: statistics-centre-abu-dhabi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scad.ae\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 08:49:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: scad.ae\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/statistics-centre-abu-dhabi/security/statistics-centre-abu-dhabi-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Statistics
- Government
- Data
- AbuDhabi
---
