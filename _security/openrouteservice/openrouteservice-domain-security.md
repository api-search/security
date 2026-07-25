---
api_specs:
- filename: openrouteservice-directions-api-openapi.yml
  format: yaml
  label: OpenRouteService Directions API
  slug: openrouteservice-directions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-directions-api-openapi.yml
- filename: openrouteservice-elevation-api-openapi.yml
  format: yaml
  label: OpenRouteService Elevation API
  slug: openrouteservice-elevation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-elevation-api-openapi.yml
- filename: openrouteservice-geocoding-api-openapi.yml
  format: yaml
  label: OpenRouteService Geocoding API
  slug: openrouteservice-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-geocoding-api-openapi.yml
- filename: openrouteservice-health-api-openapi.yml
  format: yaml
  label: OpenRouteService Health API
  slug: openrouteservice-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-health-api-openapi.yml
- filename: openrouteservice-isochrones-api-openapi.yml
  format: yaml
  label: OpenRouteService Isochrones API
  slug: openrouteservice-isochrones-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-isochrones-api-openapi.yml
- filename: openrouteservice-matrix-api-openapi.yml
  format: yaml
  label: OpenRouteService Matrix API
  slug: openrouteservice-matrix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-matrix-api-openapi.yml
- filename: openrouteservice-optimization-api-openapi.yml
  format: yaml
  label: OpenRouteService Optimization API
  slug: openrouteservice-optimization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-optimization-api-openapi.yml
- filename: openrouteservice-poi-api-openapi.yml
  format: yaml
  label: OpenRouteService POI API
  slug: openrouteservice-poi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-poi-api-openapi.yml
- filename: openrouteservice-snapping-api-openapi.yml
  format: yaml
  label: OpenRouteService Snapping API
  slug: openrouteservice-snapping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/openapi/openrouteservice-snapping-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openrouteservice.org
  spf: false
hosts:
- cert_expires: Sep 29 19:46:29 2026 GMT
  host: openrouteservice.org
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 19:17:01 2026 GMT
  host: api.openrouteservice.org
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Openrouteservice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenRouteService, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: OpenRouteService
provider_slug: openrouteservice
slug: openrouteservice-domain-security
source_filename: openrouteservice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openrouteservice.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 19:46:29 2026 GMT\n  hsts: false\n- host: api.openrouteservice.org\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  9 19:17:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: openrouteservice.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openrouteservice/refs/heads/main/security/openrouteservice-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Routing
- Geospatial
- Directions
- Isochrones
- Matrix
- Geocoding
- Elevation
- Optimization
- OpenStreetMap
- Navigation
- Logistics
- Humanitarian
---
