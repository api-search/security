---
api_specs:
- filename: google-maps-pollen-forecast-api-openapi.yml
  format: yaml
  label: Google Maps Platform Maps Pollen Forecast API
  slug: google-maps-pollen-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-pollen-forecast-api-openapi.yml
- filename: google-maps-address-validation-v1-api-openapi.yml
  format: yaml
  label: Google Maps Platform Address Validation V1 API
  slug: google-maps-address-validation-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-address-validation-v1-api-openapi.yml
- filename: google-maps-air-quality-currentconditions-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality CurrentConditions API
  slug: google-maps-air-quality-currentconditions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-currentconditions-api-openapi.yml
- filename: google-maps-air-quality-forecast-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality Forecast API
  slug: google-maps-air-quality-forecast-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-forecast-api-openapi.yml
- filename: google-maps-air-quality-history-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality History API
  slug: google-maps-air-quality-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-history-api-openapi.yml
- filename: google-maps-air-quality-maptypes-api-openapi.yml
  format: yaml
  label: Google Maps Platform Air Quality MapTypes API
  slug: google-maps-air-quality-maptypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-air-quality-maptypes-api-openapi.yml
- filename: google-maps-area-insights-v1-api-openapi.yml
  format: yaml
  label: Google Maps Platform Area Insights V1 API
  slug: google-maps-area-insights-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-area-insights-v1-api-openapi.yml
- filename: google-maps-pollen-maptypes-api-openapi.yml
  format: yaml
  label: Google Maps Platform Pollen MapTypes API
  slug: google-maps-pollen-maptypes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-pollen-maptypes-api-openapi.yml
- filename: google-maps-solar-buildinginsights-api-openapi.yml
  format: yaml
  label: Google Maps Platform Solar BuildingInsights API
  slug: google-maps-solar-buildinginsights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-solar-buildinginsights-api-openapi.yml
- filename: google-maps-solar-datalayers-api-openapi.yml
  format: yaml
  label: Google Maps Platform Solar DataLayers API
  slug: google-maps-solar-datalayers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-solar-datalayers-api-openapi.yml
- filename: google-maps-solar-geotiff-api-openapi.yml
  format: yaml
  label: Google Maps Platform Solar GeoTiff API
  slug: google-maps-solar-geotiff-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-solar-geotiff-api-openapi.yml
- filename: google-maps-street-view-publish-photo-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish Photo API
  slug: google-maps-street-view-publish-photo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photo-api-openapi.yml
- filename: google-maps-street-view-publish-photos-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish Photos API
  slug: google-maps-street-view-publish-photos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photos-api-openapi.yml
- filename: google-maps-street-view-publish-photosequence-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish PhotoSequence API
  slug: google-maps-street-view-publish-photosequence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photosequence-api-openapi.yml
- filename: google-maps-street-view-publish-photosequences-api-openapi.yml
  format: yaml
  label: Google Maps Platform Street View Publish PhotoSequences API
  slug: google-maps-street-view-publish-photosequences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/google-maps/openapi/google-maps-street-view-publish-photosequences-api-openapi.yml
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
- cert_expires: Dec 30 19:07:41 2026 GMT
  host: mapsplatform.google.com
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
name: Google Maps Platform Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Google Maps Platform, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Google Maps Platform
provider_slug: google-maps
slug: google-maps-domain-security
source_filename: google-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mapsplatform.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: false\n- host: developers.google.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:07:41 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: mapstools.googleapis.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 19:09:10 2026 GMT\n  hsts: null\ndomains:\n- domain: google.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: googleapis.com\n  dnssec: false\n  caa:\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
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
