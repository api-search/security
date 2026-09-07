---
api_specs:
- filename: aaravunmannedsystems-tile-server-openapi-original.json
  format: json
  label: Aereo Cloud Tile Server
  slug: aaravunmannedsystems-tile-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-tile-server-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aereo.io
  spf: true
hosts:
- cert_expires: Oct 10 23:49:57 2026 GMT
  host: aereo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 12 23:59:59 2026 GMT
  host: cloud.aereo.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar 18 23:59:59 2027 GMT
  host: tiles.aereo.io
  hsts: true
  hsts_max_age: 3600
  hsts_note: Corrected from the automated probe (which recorded null) by direct header inspection on 2026-09-05. max-age=3600 is one hour, far below the 31536000 normally considered effective.
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Aaravunmannedsystems Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aarav Unmanned Systems (Aereo), probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aarav Unmanned Systems (Aereo)
provider_slug: aaravunmannedsystems
slug: aaravunmannedsystems-domain-security
source_filename: aaravunmannedsystems-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aereo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 23:49:57 2026 GMT\n  hsts: false\n- host: cloud.aereo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:59:59 2026 GMT\n  hsts: false\n- host: tiles.aereo.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 18 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 3600\n  hsts_note: >-\n    Corrected from the automated probe (which recorded null) by direct header inspection on\n    2026-09-05. max-age=3600 is one hour, far below the 31536000 normally considered effective.\ndomains:\n- domain: aereo.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/security/aaravunmannedsystems-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Drones
- UAV
- Geospatial
- Mapping
- Remote Sensing
- Surveying
- Mining
- Agriculture
- Satellite Imagery
- Analytics
- India
---
