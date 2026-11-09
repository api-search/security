---
api_specs:
- filename: google-maps-autocomplete-api-openapi.yml
  format: yaml
  label: Google Maps Platform Autocomplete API
  slug: google-maps-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-autocomplete-api-openapi.yml
- filename: google-maps-directions-api-openapi.yml
  format: yaml
  label: Google Maps Platform Directions API
  slug: google-maps-directions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-directions-api-openapi.yml
- filename: google-maps-geocoding-api-openapi.yml
  format: yaml
  label: Google Maps Platform Geocoding API
  slug: google-maps-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-geocoding-api-openapi.yml
- filename: google-maps-nearby-search-api-openapi.yml
  format: yaml
  label: Google Maps Platform Nearby Search API
  slug: google-maps-nearby-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-nearby-search-api-openapi.yml
- filename: google-maps-photos-api-openapi.yml
  format: yaml
  label: Google Maps Platform Photos API
  slug: google-maps-photos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-photos-api-openapi.yml
- filename: google-maps-place-details-api-openapi.yml
  format: yaml
  label: Google Maps Platform Place Details API
  slug: google-maps-place-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-place-details-api-openapi.yml
- filename: google-maps-text-search-api-openapi.yml
  format: yaml
  label: Google Maps Platform Text Search API
  slug: google-maps-text-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-text-search-api-openapi.yml
- filename: google-maps-directions-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Directions API
  slug: google-maps-directions-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-directions-api-api-openapi.yml
- filename: google-maps-distance-matrix-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Distance Matrix API
  slug: google-maps-distance-matrix-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-distance-matrix-api-api-openapi.yml
- filename: google-maps-elevation-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Elevation API
  slug: google-maps-elevation-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-elevation-api-api-openapi.yml
- filename: google-maps-geocoding-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Geocoding API
  slug: google-maps-geocoding-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-geocoding-api-api-openapi.yml
- filename: google-maps-geolocation-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Geolocation API
  slug: google-maps-geolocation-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-geolocation-api-api-openapi.yml
- filename: google-maps-places-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Places API
  slug: google-maps-places-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-places-api-api-openapi.yml
- filename: google-maps-roads-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Roads API
  slug: google-maps-roads-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-roads-api-api-openapi.yml
- filename: google-maps-street-view-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View API
  slug: google-maps-street-view-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-api-api-openapi.yml
- filename: google-maps-time-zone-api-api-openapi.yml
  format: yaml
  label: Google Maps Platform Time Zone API
  slug: google-maps-time-zone-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-time-zone-api-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: google.com
  spf: true
- caa:
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: googleapis.com
  spf: true
hosts:
- cert_expires: Dec 30 19:09:53 2026 GMT
  host: www.google.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: developers.google.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 19:09:10 2026 GMT
  host: mapstools.googleapis.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Google Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Maps Platform, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Maps Platform
provider_slug: google-maps
slug: google-maps-domain-security
source_filename: google-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:53 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mapstools.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/google-maps/security/google-maps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Environment
- Geocoding
- Geolocation
- Maps
- Navigation
- Places
- Routing
- Solar
- Geospatial
---
