---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: witricity.com
  spf: true
hosts:
- cert_expires: Oct  3 12:49:00 2026 GMT
  host: www.witricity.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Witricity Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WiTricity, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: WiTricity
provider_slug: witricity
slug: witricity-domain-security
source_filename: witricity-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.witricity.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 12:49:00 2026 GMT\n  hsts: false\ndomains:\n- domain: witricity.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/witricity/refs/heads/main/security/witricity-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Wireless Power
- Electric Vehicles
- EV Charging
- Automotive
- Energy
- Hardware
- Intellectual Property Licensing
- Smart Cities
- Vehicle to Grid
---
