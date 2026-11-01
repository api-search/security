---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gc.ca
  spf: true
hosts:
- cert_expires: May  5 23:59:59 2027 GMT
  host: www.nrcan.gc.ca
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Geoconnections Natural Resources Canada Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GeoConnections - Natural Resources Canada, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: GeoConnections - Natural Resources Canada
provider_slug: geoconnections-natural-resources-canada
slug: geoconnections-natural-resources-canada-domain-security
source_filename: geoconnections-natural-resources-canada-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.nrcan.gc.ca\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: May  5 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: gc.ca\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/geoconnections-natural-resources-canada/security/geoconnections-natural-resources-canada-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Government
- Natural Resources
- Canada
- Geospatial Data
- Sustainability
---
