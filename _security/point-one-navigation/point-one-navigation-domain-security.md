---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: pointonenav.com
  spf: true
hosts:
- cert_expires: Sep  7 12:45:29 2026 GMT
  host: pointonenav.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 05:19:54 2026 GMT
  host: support.pointonenav.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 15 00:16:41 2026 GMT
  host: api.pointonenav.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Point One Navigation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Point One Navigation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Point One Navigation
provider_slug: point-one-navigation
slug: point-one-navigation-domain-security
source_filename: point-one-navigation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pointonenav.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 12:45:29 2026 GMT\n  hsts: false\n- host: support.pointonenav.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 05:19:54 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.pointonenav.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 00:16:41 2026 GMT\n  hsts: false\ndomains:\n- domain: pointonenav.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/point-one-navigation/refs/heads/main/security/point-one-navigation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Location
- GNSS
- Positioning
- Geospatial
- RTK
- Navigation
- Mapping
- Robotics
- Autonomous Vehicles
- IoT
- Hardware
- GraphQL
---
