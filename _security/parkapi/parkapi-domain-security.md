---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: parkendd.de
  spf: false
hosts:
- cert_expires: Jan 23 14:57:47 2027 GMT
  host: parkendd.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: ParkenDD Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ParkenDD, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: ParkenDD
provider_slug: parkapi
slug: parkapi-domain-security
source_filename: parkapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: parkendd.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 14:57:47 2027 GMT\n  hsts: false\ndomains:\n- domain: parkendd.de\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/parkapi/security/parkapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Parking
- Real-Time
- Europe
- Mobile
- Open Data
---
