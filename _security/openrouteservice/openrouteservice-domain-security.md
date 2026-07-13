---
api_specs:
- filename: ors
  format: yaml
  label: OpenRouteService Directions API
  slug: directions
  spec_type: OpenAPI
  url: https://openrouteservice.org/wp-json/ors
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
