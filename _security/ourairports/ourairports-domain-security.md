---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: ourairports.com
  spf: false
hosts:
- cert_expires: Oct 10 15:21:45 2026 GMT
  host: ourairports.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ourairports Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OurAirports, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OurAirports
provider_slug: ourairports
slug: ourairports-domain-security
source_filename: ourairports-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ourairports.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 15:21:45 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ourairports.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ourairports/refs/heads/main/security/ourairports-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Aviation
- Airports
- Open Data
- CSV
- Geospatial
- Transportation
- Runways
- Navaids
- Public Domain
---
