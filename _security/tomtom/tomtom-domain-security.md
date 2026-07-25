---
api_specs:
- filename: tomtom-geocoding-api-openapi.yml
  format: yaml
  label: TomTom Geocoding API
  slug: tomtom-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-geocoding-api-openapi.yml
- filename: tomtom-additional-data-api-openapi.yml
  format: yaml
  label: TomTom Additional Data API
  slug: tomtom-additional-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-additional-data-api-openapi.yml
- filename: tomtom-batch-routing-api-openapi.yml
  format: yaml
  label: TomTom Batch Routing API
  slug: tomtom-batch-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-batch-routing-api-openapi.yml
- filename: tomtom-copyrights-api-openapi.yml
  format: yaml
  label: TomTom Copyrights API
  slug: tomtom-copyrights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-copyrights-api-openapi.yml
- filename: tomtom-filters-api-openapi.yml
  format: yaml
  label: TomTom Filters API
  slug: tomtom-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-filters-api-openapi.yml
- filename: tomtom-geocoding-api-openapi.yml
  format: yaml
  label: TomTom Geocoding API
  slug: tomtom-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-geocoding-api-openapi.yml
- filename: tomtom-raster-api-openapi.yml
  format: yaml
  label: TomTom Raster API
  slug: tomtom-raster-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-raster-api-openapi.yml
- filename: tomtom-reachable-range-api-openapi.yml
  format: yaml
  label: TomTom Reachable Range API
  slug: tomtom-reachable-range-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-reachable-range-api-openapi.yml
- filename: tomtom-reverse-geocoding-api-openapi.yml
  format: yaml
  label: TomTom Reverse Geocoding API
  slug: tomtom-reverse-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-reverse-geocoding-api-openapi.yml
- filename: tomtom-routing-api-openapi.yml
  format: yaml
  label: TomTom Routing API
  slug: tomtom-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-routing-api-openapi.yml
- filename: tomtom-search-api-openapi.yml
  format: yaml
  label: TomTom Search API
  slug: tomtom-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-search-api-openapi.yml
- filename: tomtom-traffic-flow-api-openapi.yml
  format: yaml
  label: TomTom Traffic Flow API
  slug: tomtom-traffic-flow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-traffic-flow-api-openapi.yml
- filename: tomtom-traffic-incidents-api-openapi.yml
  format: yaml
  label: TomTom Traffic Incidents API
  slug: tomtom-traffic-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-traffic-incidents-api-openapi.yml
- filename: tomtom-traffic-tiles-api-openapi.yml
  format: yaml
  label: TomTom Traffic Tiles API
  slug: tomtom-traffic-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-traffic-tiles-api-openapi.yml
- filename: tomtom-vector-api-openapi.yml
  format: yaml
  label: TomTom Vector API
  slug: tomtom-vector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-vector-api-openapi.yml
- filename: tomtom-wms-wmts-api-openapi.yml
  format: yaml
  label: TomTom WMS / WMTS API
  slug: tomtom-wms-wmts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/openapi/tomtom-wms-wmts-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tomtom.com
  spf: true
hosts:
- cert_expires: Oct 11 10:30:23 2026 GMT
  host: www.tomtom.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 11 10:30:23 2026 GMT
  host: developer.tomtom.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 17 10:15:00 2026 GMT
  host: api.tomtom.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tomtom Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for TomTom, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: TomTom
provider_slug: tomtom
slug: tomtom-domain-security
source_filename: tomtom-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tomtom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 10:30:23 2026 GMT\n  hsts: false\n- host: developer.tomtom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 10:30:23 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.tomtom.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 17 10:15:00 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: tomtom.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tomtom/refs/heads/main/security/tomtom-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Maps
- Traffic
- Transportation
- Navigation
- Location
- Geospatial
- Routing
- Geocoding
---
