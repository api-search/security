---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: advancednavigation.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: advancednavigation.com.au
  spf: true
hosts:
- cert_expires: Nov  2 09:31:58 2026 GMT
  host: www.advancednavigation.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 19 23:59:59 2027 GMT
  host: hq.advancednavigation.com.au
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Advancednavigation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Advanced Navigation, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: Advanced Navigation
provider_slug: advancednavigation
slug: advancednavigation-domain-security
source_filename: advancednavigation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.advancednavigation.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  2 09:31:58 2026 GMT\n  hsts: false\n- host: hq.advancednavigation.com.au\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 19 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: advancednavigation.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n- domain: advancednavigation.com.au\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/advancednavigation/refs/heads/main/security/advancednavigation-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Navigation
- Inertial Navigation
- GNSS
- Positioning
- Robotics
- Defense
- Subsea
- Geospatial
- Post Processing
- Hardware
---
