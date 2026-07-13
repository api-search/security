---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Valhalla Route API
  slug: valhalla-route-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Optimized Route API
  slug: valhalla-optimized-route-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Matrix API
  slug: valhalla-matrix-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Isochrone API
  slug: valhalla-isochrone-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Map Matching API
  slug: valhalla-map-matching-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Elevation API
  slug: valhalla-elevation-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Expansion API
  slug: valhalla-expansion-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Locate API
  slug: valhalla-locate-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Status API
  slug: valhalla-status-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openstreetmap.de
  spf: true
hosts:
- cert_expires: Oct  3 20:09:52 2026 GMT
  host: valhalla1.openstreetmap.de
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Valhalla Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Valhalla, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Valhalla
provider_slug: valhalla
slug: valhalla-domain-security
source_filename: valhalla-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: valhalla1.openstreetmap.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 20:09:52 2026 GMT\n  hsts: null\ndomains:\n- domain: openstreetmap.de\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valhalla/refs/heads/main/security/valhalla-domain-security.yml
summary_line: TLSv1.3
tags:
- Routing
- Navigation
- OpenStreetMap
- Mapping
- Geospatial
- Directions
- Isochrones
- Travel
- Transportation
- Open Source
---
