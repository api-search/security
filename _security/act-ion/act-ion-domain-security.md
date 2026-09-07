---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: act-ion.com
  spf: true
hosts:
- cert_expires: Nov 27 07:17:28 2026 GMT
  host: www.act-ion.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Act Ion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACT-ion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: ACT-ion
provider_slug: act-ion
slug: act-ion-domain-security
source_filename: act-ion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.act-ion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 07:17:28 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: act-ion.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/act-ion/refs/heads/main/security/act-ion-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Energy
- Battery Materials
- Cathode Active Materials
- Lithium-Ion Batteries
- Energy Storage
- Advanced Manufacturing
- Clean Energy
- Electric Vehicles
- Materials Science
- Deep Tech
- Texas
---
