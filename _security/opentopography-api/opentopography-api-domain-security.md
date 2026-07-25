---
api_specs:
- filename: opentopography-api-public-api-openapi.yml
  format: yaml
  label: OpenTopography API Public API
  slug: opentopography-api-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/opentopography-api/refs/heads/main/openapi/opentopography-api-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: opentopography.org
  spf: false
hosts:
- cert_expires: Aug 30 14:51:04 2026 GMT
  host: opentopography.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 25 09:31:36 2026 GMT
  host: portal.opentopography.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Opentopography Api Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenTopography API, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: OpenTopography API
provider_slug: opentopography-api
slug: opentopography-api-domain-security
source_filename: opentopography-api-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: opentopography.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 30 14:51:04 2026 GMT\n  hsts: false\n- host: portal.opentopography.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 09:31:36 2026 GMT\n  hsts: false\ndomains:\n- domain: opentopography.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/opentopography-api/refs/heads/main/security/opentopography-api-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- DEM
- Data
- Elevation
- Geospatial
- LiDAR
- Topographical
- Topography
---
