---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agiindia.com
  spf: true
hosts:
- cert_expires: Dec 22 06:25:39 2026 GMT
  host: agiindia.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Association Of Geospatial Industries Agi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Association of Geospatial Industries (AGI), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Association of Geospatial Industries (AGI)
provider_slug: association-of-geospatial-industries-agi
slug: association-of-geospatial-industries-agi-domain-security
source_filename: association-of-geospatial-industries-agi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agiindia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 06:25:39 2026 GMT\n  hsts: null\ndomains:\n- domain: agiindia.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/association-of-geospatial-industries-agi/security/association-of-geospatial-industries-agi-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geospatial
- Industry Association
- GIS
- Remote Sensing
- Drone Survey
- LiDAR
- Cloud Computing
- Policy
---
