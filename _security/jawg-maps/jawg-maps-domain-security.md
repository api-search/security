---
api_specs:
- filename: jawg-maps-openapi.yml
  format: yaml
  label: Jawg Map Tiles & Styles API
  slug: jawg-maps-map-tiles-styles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-openapi.yml
- filename: jawg-maps-openapi.yml
  format: yaml
  label: Jawg Places / Geocoding API
  slug: jawg-maps-places-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-openapi.yml
- filename: jawg-maps-openapi.yml
  format: yaml
  label: Jawg Routing API
  slug: jawg-maps-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-openapi.yml
- filename: jawg-maps-openapi.yml
  format: yaml
  label: Jawg Matrix API
  slug: jawg-maps-matrix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-openapi.yml
- filename: jawg-maps-openapi.yml
  format: yaml
  label: Jawg Isochrone API
  slug: jawg-maps-isochrone-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-openapi.yml
- filename: jawg-maps-openapi.yml
  format: yaml
  label: Jawg Static Maps API
  slug: jawg-maps-static-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/openapi/jawg-maps-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "letsencrypt.org;validationmethods=dns-01"
  - 0 iodef "mailto:tls-abuse@jawg.io"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: jawg.io
  spf: false
hosts:
- cert_expires: Sep  9 20:25:27 2026 GMT
  host: www.jawg.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 11:06:09 2026 GMT
  host: tile.jawg.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  7 11:06:09 2026 GMT
  host: api.jawg.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Jawg Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Jawg Maps, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: Jawg Maps
provider_slug: jawg-maps
slug: jawg-maps-domain-security
source_filename: jawg-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.jawg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 20:25:27 2026 GMT\n  hsts: false\n- host: tile.jawg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:06:09 2026 GMT\n  hsts: null\n- host: api.jawg.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 11:06:09 2026 GMT\n  hsts: null\ndomains:\n- domain: jawg.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"letsencrypt.org;validationmethods=dns-01\"\n  - 0 iodef \"mailto:tls-abuse@jawg.io\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jawg-maps/refs/heads/main/security/jawg-maps-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Maps
- Geospatial
- Tiles
- Geocoding
- Routing
- Location
---
