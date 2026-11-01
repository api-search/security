---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: uni-lj.si
  spf: true
hosts:
- cert_expires: Jan 16 01:08:14 2027 GMT
  host: www.en.fgg.uni-lj.si
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: University Of Ljubljana Faculty Of Civil And Geodetic Engineering Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for University of Ljubljana, Faculty of Civil and Geodetic Engineering, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: University of Ljubljana, Faculty of Civil and Geodetic Engineering
provider_slug: university-of-ljubljana-faculty-of-civil-and-geodetic-engineering
slug: university-of-ljubljana-faculty-of-civil-and-geodetic-engineering-domain-security
source_filename: university-of-ljubljana-faculty-of-civil-and-geodetic-engineering-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.en.fgg.uni-lj.si\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 01:08:14 2027 GMT\n  hsts: false\ndomains:\n- domain: uni-lj.si\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/university-of-ljubljana-faculty-of-civil-and-geodetic-engineering/security/university-of-ljubljana-faculty-of-civil-and-geodetic-engineering-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Education
- Research
- Civil Engineering
- Geodesy
- Academia
---
