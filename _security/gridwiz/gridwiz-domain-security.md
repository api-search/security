---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: gridwiz.com
  spf: true
hosts:
- cert_expires: Dec 26 05:47:16 2026 GMT
  host: www.gridwiz.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Gridwiz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gridwiz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Gridwiz
provider_slug: gridwiz
slug: gridwiz-domain-security
source_filename: gridwiz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.gridwiz.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 26 05:47:16 2026 GMT\n  hsts: false\ndomains:\n- domain: gridwiz.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gridwiz/refs/heads/main/security/gridwiz-domain-security.yml
summary_line: TLSv1.2
tags:
- Company
- Energy
- Demand Response
- Electric Vehicles
- EV Charging
- Smart Grid
- Energy Storage
- Renewable Energy
- Vehicle to Grid
- South Korea
---
