---
api_specs:
- filename: stadia-maps-attributes-api-openapi.yml
  format: yaml
  label: Stadia Maps Attributes API
  slug: stadia-maps-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-attributes-api-openapi.yml
- filename: stadia-maps-autocomplete-api-openapi.yml
  format: yaml
  label: Stadia Maps Autocomplete API
  slug: stadia-maps-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-autocomplete-api-openapi.yml
- filename: stadia-maps-geospatial-api-openapi.yml
  format: yaml
  label: Stadia Maps Geospatial API
  slug: stadia-maps-geospatial-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-geospatial-api-openapi.yml
- filename: stadia-maps-lookups-api-openapi.yml
  format: yaml
  label: Stadia Maps Lookups API
  slug: stadia-maps-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-lookups-api-openapi.yml
- filename: stadia-maps-match-api-openapi.yml
  format: yaml
  label: Stadia Maps Match API
  slug: stadia-maps-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-match-api-openapi.yml
- filename: stadia-maps-place-api-openapi.yml
  format: yaml
  label: Stadia Maps Place API
  slug: stadia-maps-place-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-place-api-openapi.yml
- filename: stadia-maps-reverse-api-openapi.yml
  format: yaml
  label: Stadia Maps Reverse API
  slug: stadia-maps-reverse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-reverse-api-openapi.yml
- filename: stadia-maps-roads-api-openapi.yml
  format: yaml
  label: Stadia Maps Roads API
  slug: stadia-maps-roads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-roads-api-openapi.yml
- filename: stadia-maps-routes-api-openapi.yml
  format: yaml
  label: Stadia Maps Routes API
  slug: stadia-maps-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-routes-api-openapi.yml
- filename: stadia-maps-routing-api-openapi.yml
  format: yaml
  label: Stadia Maps Routing API
  slug: stadia-maps-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-routing-api-openapi.yml
- filename: stadia-maps-search-api-openapi.yml
  format: yaml
  label: Stadia Maps Search API
  slug: stadia-maps-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/openapi/stadia-maps-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: stadiamaps.com
  spf: true
hosts:
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: stadiamaps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: docs.stadiamaps.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 28 23:59:59 2026 GMT
  host: api.stadiamaps.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Stadia Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stadia Maps, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Stadia Maps
provider_slug: stadia-maps
slug: stadia-maps-domain-security
source_filename: stadia-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stadiamaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.stadiamaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.stadiamaps.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 28 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: stadiamaps.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stadia-maps/refs/heads/main/security/stadia-maps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Mapping
- Maps
- Geocoding
- Routing
- Navigation
- Geospatial
- Location
---
