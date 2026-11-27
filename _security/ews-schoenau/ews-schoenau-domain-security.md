---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: ews-schoenau.de
  spf: true
hosts:
- cert_expires: Jan 23 01:46:20 2027 GMT
  host: ews-schoenau.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EWS Elektrizitaetswerke Schoenau Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EWS Elektrizitaetswerke Schoenau, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: EWS Elektrizitaetswerke Schoenau
provider_slug: ews-schoenau
slug: ews-schoenau-domain-security
source_filename: ews-schoenau-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ews-schoenau.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 01:46:20 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ews-schoenau.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/ews-schoenau/security/ews-schoenau-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Energy
- Renewables
- Cooperative
- Germany
---
