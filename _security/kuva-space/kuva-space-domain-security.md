---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: kuvaspace.com
  spf: true
hosts:
- cert_expires: Aug 24 07:44:16 2026 GMT
  host: kuvaspace.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kuva Space Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kuva Space, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Kuva Space
provider_slug: kuva-space
slug: kuva-space-domain-security
source_filename: kuva-space-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kuvaspace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 07:44:16 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: kuvaspace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kuva-space/refs/heads/main/security/kuva-space-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Earth Observation
- Hyperspectral Imaging
- Satellite Imagery
- Remote Sensing
- Microsatellites
- CubeSat
- Space
- Geospatial
- Planetary Intelligence
- Agriculture
- Aquaculture
- Environment
- Carbon Monitoring
- Deforestation
- Maritime Domain Awareness
- Safety And Security
- Crisis Response
- Climate
- AI
- Insights As A Service
- Finland
- Nordic Space
- ESA InCubed
- Hyperfield
- Kuva Sense
---
