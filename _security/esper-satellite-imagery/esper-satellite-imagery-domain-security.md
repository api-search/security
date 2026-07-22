---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: espersatellites.co
  spf: true
hosts:
- cert_expires: Sep 23 08:14:41 2026 GMT
  host: espersatellites.co
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Esper Satellite Imagery Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Esper Satellite Imagery, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Esper Satellite Imagery
provider_slug: esper-satellite-imagery
slug: esper-satellite-imagery-domain-security
source_filename: esper-satellite-imagery-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: espersatellites.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 08:14:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: espersatellites.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esper-satellite-imagery/refs/heads/main/security/esper-satellite-imagery-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Satellite Imagery
- Hyperspectral
- Earth Observation
- Remote Sensing
- Mineral Exploration
- Geospatial
- Space
---
