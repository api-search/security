---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hei.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: hawaiianelectric.com
  spf: true
hosts:
- cert_expires: Dec  7 22:10:50 2026 GMT
  host: www.hei.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  8 23:59:59 2027 GMT
  host: www.hawaiianelectric.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 13 23:59:59 2026 GMT
  host: services5.arcgis.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Hawaiian Electric Industries Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hawaiian Electric Industries, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Hawaiian Electric Industries
provider_slug: hawaiian-electric-industries
slug: hawaiian-electric-industries-domain-security
source_filename: hawaiian-electric-industries-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hei.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 22:10:50 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.hawaiianelectric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  8 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: services5.arcgis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hei.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: hawaiianelectric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hawaiian-electric-industries/refs/heads/main/security/hawaiian-electric-industries-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Energy
- Utilities
- Electricity
- Grid
- Holding Company
- Hawaii
- Fortune 1000
- Geospatial
- ArcGIS
- Open Data
- Locational Value Map
- EV Charging
---
