---
api_specs:
- filename: microsoft-azure-maps-search-api-openapi.yml
  format: yaml
  label: Azure Maps Search API
  slug: microsoft-azure-maps-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-search-api-openapi.yml
- filename: microsoft-azure-maps-geocode-api-openapi.yml
  format: yaml
  label: Azure Maps Geocode API
  slug: microsoft-azure-maps-geocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geocode-api-openapi.yml
- filename: microsoft-azure-maps-geocode-autocomplete-api-openapi.yml
  format: yaml
  label: Azure Maps Geocode:autocomplete API
  slug: microsoft-azure-maps-geocode-autocomplete-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geocode-autocomplete-api-openapi.yml
- filename: microsoft-azure-maps-geocode-batch-api-openapi.yml
  format: yaml
  label: Azure Maps Geocode:batch API
  slug: microsoft-azure-maps-geocode-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geocode-batch-api-openapi.yml
- filename: microsoft-azure-maps-geolocation-api-openapi.yml
  format: yaml
  label: Azure Maps Geolocation API
  slug: microsoft-azure-maps-geolocation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-geolocation-api-openapi.yml
- filename: microsoft-azure-maps-map-api-openapi.yml
  format: yaml
  label: Azure Maps Map API
  slug: microsoft-azure-maps-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-map-api-openapi.yml
- filename: microsoft-azure-maps-reversegeocode-api-openapi.yml
  format: yaml
  label: Azure Maps Reverse Geocode API
  slug: microsoft-azure-maps-reversegeocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-reversegeocode-api-openapi.yml
- filename: microsoft-azure-maps-reversegeocode-batch-api-openapi.yml
  format: yaml
  label: Azure Maps Reverse Geocode:batch API
  slug: microsoft-azure-maps-reversegeocode-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-reversegeocode-batch-api-openapi.yml
- filename: microsoft-azure-maps-route-api-openapi.yml
  format: yaml
  label: Azure Maps Route API
  slug: microsoft-azure-maps-route-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-route-api-openapi.yml
- filename: microsoft-azure-maps-timezone-api-openapi.yml
  format: yaml
  label: Azure Maps Timezone API
  slug: microsoft-azure-maps-timezone-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-timezone-api-openapi.yml
- filename: microsoft-azure-maps-traffic-api-openapi.yml
  format: yaml
  label: Azure Maps Traffic API
  slug: microsoft-azure-maps-traffic-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-traffic-api-openapi.yml
- filename: microsoft-azure-maps-weather-api-openapi.yml
  format: yaml
  label: Azure Maps Weather API
  slug: microsoft-azure-maps-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-weather-api-openapi.yml
- filename: microsoft-azure-maps-accounts-api-openapi.yml
  format: yaml
  label: Azure Maps Accounts API
  slug: microsoft-azure-maps-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-accounts-api-openapi.yml
- filename: microsoft-azure-maps-creators-api-openapi.yml
  format: yaml
  label: Azure Maps Creators API
  slug: microsoft-azure-maps-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-creators-api-openapi.yml
- filename: microsoft-azure-maps-operations-api-openapi.yml
  format: yaml
  label: Azure Maps Operations API
  slug: microsoft-azure-maps-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-azure-maps/openapi/microsoft-azure-maps-operations-api-openapi.yml
description: ''
domains:
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: azure.com
  spf: true
- caa:
  - 0 contactemail "caarecordaware@microsoft.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: microsoft.com
  spf: true
hosts:
- cert_expires: Jan 21 18:52:15 2027 GMT
  host: portal.azure.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  2 19:05:38 2027 GMT
  host: azure.microsoft.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Apr  8 00:23:13 2027 GMT
  host: learn.microsoft.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Azure Maps Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Azure Maps, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Azure Maps
provider_slug: microsoft-azure-maps
slug: microsoft-azure-maps-domain-security
source_filename: microsoft-azure-maps-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: portal.azure.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 18:52:15 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: azure.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  2 19:05:38 2027 GMT\n  hsts: null\n- host: learn.microsoft.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Apr  8 00:23:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: azure.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: microsoft.com\n  dnssec: false\n  caa:\n  - 0 contactemail \"caarecordaware@microsoft.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/microsoft-azure-maps/security/microsoft-azure-maps-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Geocoding
- Geospatial
- Location
- Maps
- Mobility
- Routing
- Traffic
- Weather
---
