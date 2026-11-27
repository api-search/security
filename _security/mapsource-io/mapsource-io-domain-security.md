---
api_specs:
- filename: mapsource-io-account-api-openapi.yml
  format: yaml
  label: Mapsource Account API
  slug: mapsource-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-account-api-openapi.yml
- filename: mapsource-io-cartography-api-openapi.yml
  format: yaml
  label: Mapsource Cartography API
  slug: mapsource-io-cartography-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-cartography-api-openapi.yml
- filename: mapsource-io-compute-api-openapi.yml
  format: yaml
  label: Mapsource Compute API
  slug: mapsource-io-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-compute-api-openapi.yml
- filename: mapsource-io-delivery-api-openapi.yml
  format: yaml
  label: Mapsource Delivery API
  slug: mapsource-io-delivery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-delivery-api-openapi.yml
- filename: mapsource-io-discovery-api-openapi.yml
  format: yaml
  label: Mapsource Discovery API
  slug: mapsource-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-discovery-api-openapi.yml
- filename: mapsource-io-meta-api-openapi.yml
  format: yaml
  label: Mapsource Meta API
  slug: mapsource-io-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-meta-api-openapi.yml
- filename: mapsource-io-navigation-api-openapi.yml
  format: yaml
  label: Mapsource Navigation API
  slug: mapsource-io-navigation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-navigation-api-openapi.yml
- filename: mapsource-io-terrain-api-openapi.yml
  format: yaml
  label: Mapsource Terrain API
  slug: mapsource-io-terrain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-terrain-api-openapi.yml
- filename: mapsource-io-weather-api-openapi.yml
  format: yaml
  label: Mapsource Weather API
  slug: mapsource-io-weather-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mapsource-io/openapi/mapsource-io-weather-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: mapsource.io
  spf: false
hosts:
- cert_expires: Jan 31 22:53:35 2027 GMT
  host: mapsource.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mapsource Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mapsource, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Mapsource
provider_slug: mapsource-io
slug: mapsource-io-domain-security
source_filename: mapsource-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mapsource.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 31 22:53:35 2027 GMT\n  hsts: false\ndomains:\n- domain: mapsource.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mapsource-io/security/mapsource-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Geospatial
- OpenStreetMap
- Mapping
- Cloud
---
