---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cellinktechnologies.com
  spf: true
hosts:
- cert_expires: Sep 26 09:14:44 2026 GMT
  host: cellinktechnologies.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cellink Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CelLink, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CelLink
provider_slug: cellink
slug: cellink-domain-security
source_filename: cellink-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cellinktechnologies.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 09:14:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cellinktechnologies.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cellink/refs/heads/main/security/cellink-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Manufacturing
- Electrification
- Electric Vehicles
- Flexible Circuits
- Wiring Harness
- Battery
- Data Center
- Automotive
- Hardware
---
