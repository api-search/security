---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: fgov.be
  spf: true
hosts:
- cert_expires: Feb  6 21:53:44 2027 GMT
  host: statbel.fgov.be
  hsts: true
  hsts_max_age: 1000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Statbel (Belgian statistics) Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Statbel (Belgian statistics), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Statbel (Belgian statistics)
provider_slug: statbel-be
slug: statbel-be-domain-security
source_filename: statbel-be-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: statbel.fgov.be\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 21:53:44 2027 GMT\n  hsts: true\n  hsts_max_age: 1000\ndomains:\n- domain: fgov.be\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/statbel-be/security/statbel-be-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Government
- Statistics
- Open Data
- Belgium
- Official Statistics
---
