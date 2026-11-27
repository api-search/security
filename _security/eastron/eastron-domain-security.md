---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: eastrongroup.com
  spf: true
hosts:
- cert_expires: Feb  3 13:12:04 2027 GMT
  host: eastrongroup.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Eastron Electronic Co., Ltd. Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Eastron Electronic Co., Ltd., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Eastron Electronic Co., Ltd.
provider_slug: eastron
slug: eastron-domain-security
source_filename: eastron-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eastrongroup.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 13:12:04 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eastrongroup.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/eastron/security/eastron-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Electricity Meters
- Smart Meter
- Energy Measurement
- EV Charging
- Solar PV
- Data Center
- Power Analyzer
- Load Balancing
---
