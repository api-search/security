---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: geopipe.ai
  spf: false
hosts:
- cert_expires: Aug 10 11:10:15 2026 GMT
  host: geopipe.ai
  hsts: true
  hsts_max_age: 31556952
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Geopipe Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Geopipe, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Geopipe
provider_slug: geopipe
slug: geopipe-domain-security
source_filename: geopipe-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geopipe.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 10 11:10:15 2026 GMT\n  hsts: true\n  hsts_max_age: 31556952\ndomains:\n- domain: geopipe.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geopipe/refs/heads/main/security/geopipe-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- 3D
- Digital Twins
- Geospatial
- Gaming
- Simulation
- Unity
- Unreal Engine
- Cesium
- 3D Tiles
- Metaverse
- Maps
---
