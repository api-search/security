---
api_specs:
- filename: dlr-capabilities-api-openapi.yml
  format: yaml
  label: DLR Capabilities API
  slug: dlr-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlr/refs/heads/main/openapi/dlr-capabilities-api-openapi.yml
- filename: dlr-data-api-openapi.yml
  format: yaml
  label: DLR Data API
  slug: dlr-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlr/refs/heads/main/openapi/dlr-data-api-openapi.yml
- filename: dlr-stac-api-openapi.yml
  format: yaml
  label: DLR STAC API
  slug: dlr-stac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dlr/refs/heads/main/openapi/dlr-stac-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: dlr.de
  spf: true
hosts:
- cert_expires: Oct 31 05:57:00 2026 GMT
  host: geoservice.dlr.de
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.2
- cert_expires: Sep 22 11:41:13 2026 GMT
  host: eoweb.dlr.de
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Dlr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DLR, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: DLR
provider_slug: dlr
slug: dlr-domain-security
source_filename: dlr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: geoservice.dlr.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 31 05:57:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: eoweb.dlr.de\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep 22 11:41:13 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: dlr.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dlr/refs/heads/main/security/dlr-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Earth Observation
- Remote Sensing
- Satellite Data
- Geospatial
- Aerospace
- Open Data
- OGC
- STAC
- Atmospheric Science
- Digital Elevation Models
---
