---
api_specs:
- filename: aaravunmannedsystems-3dtiles-api-openapi.yml
  format: yaml
  label: Aarav Unmanned Systems (Aereo) 3dtiles API
  slug: aaravunmannedsystems-3dtiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-3dtiles-api-openapi.yml
- filename: aaravunmannedsystems-altitude-api-openapi.yml
  format: yaml
  label: Aarav Unmanned Systems (Aereo) Altitude API
  slug: aaravunmannedsystems-altitude-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-altitude-api-openapi.yml
- filename: aaravunmannedsystems-cesium-terrain-api-openapi.yml
  format: yaml
  label: Aarav Unmanned Systems (Aereo) Cesium Terrain API
  slug: aaravunmannedsystems-cesium-terrain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-cesium-terrain-api-openapi.yml
- filename: aaravunmannedsystems-cv-tiles-api-openapi.yml
  format: yaml
  label: Aarav Unmanned Systems (Aereo) Cv Tiles API
  slug: aaravunmannedsystems-cv-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-cv-tiles-api-openapi.yml
- filename: aaravunmannedsystems-histogram-api-openapi.yml
  format: yaml
  label: Aarav Unmanned Systems (Aereo) Histogram API
  slug: aaravunmannedsystems-histogram-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-histogram-api-openapi.yml
- filename: aaravunmannedsystems-mbtiles-api-openapi.yml
  format: yaml
  label: Aarav Unmanned Systems (Aereo) Mbtiles API
  slug: aaravunmannedsystems-mbtiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-mbtiles-api-openapi.yml
- filename: aaravunmannedsystems-ortho-api-openapi.yml
  format: yaml
  label: Aarav Unmanned Systems (Aereo) Ortho API
  slug: aaravunmannedsystems-ortho-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-ortho-api-openapi.yml
- filename: aaravunmannedsystems-ping-api-openapi.yml
  format: yaml
  label: Aarav Unmanned Systems (Aereo) Ping API
  slug: aaravunmannedsystems-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-ping-api-openapi.yml
- filename: aaravunmannedsystems-terrain-api-openapi.yml
  format: yaml
  label: Aarav Unmanned Systems (Aereo) Terrain API
  slug: aaravunmannedsystems-terrain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-terrain-api-openapi.yml
- filename: aaravunmannedsystems-vector-api-openapi.yml
  format: yaml
  label: Aarav Unmanned Systems (Aereo) Vector API
  slug: aaravunmannedsystems-vector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aaravunmannedsystems/refs/heads/main/openapi/aaravunmannedsystems-vector-api-openapi.yml
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
