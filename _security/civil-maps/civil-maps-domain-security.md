---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: civilmaps.com
  spf: true
hosts:
- cert_expires: Sep 21 19:14:43 2026 GMT
  host: civilmaps.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Civil Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Civil Maps, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Civil Maps
provider_slug: civil-maps
slug: civil-maps-domain-security
source_filename: civil-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: civilmaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 19:14:43 2026 GMT\n  hsts: false\ndomains:\n- domain: civilmaps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/civil-maps/refs/heads/main/security/civil-maps-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Autonomous Vehicles
- HD Mapping
- Localization
- LiDAR
- Point Cloud
- Geospatial
- Automotive
- Machine Learning
- Acquired
- United States
---
