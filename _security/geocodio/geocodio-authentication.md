---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: geocodio-lists-api-openapi.yml
  format: yaml
  label: Geocodio Lists API
  slug: geocodio-lists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geocodio/openapi/geocodio-lists-api-openapi.yml
- filename: geocodio-distance-api-openapi.yml
  format: yaml
  label: Geocodio Distance API
  slug: geocodio-distance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geocodio/openapi/geocodio-distance-api-openapi.yml
- filename: geocodio-distance-jobs-api-openapi.yml
  format: yaml
  label: Geocodio Distance Jobs API
  slug: geocodio-distance-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geocodio/openapi/geocodio-distance-jobs-api-openapi.yml
- filename: geocodio-distance-matrix-api-openapi.yml
  format: yaml
  label: Geocodio Distance Matrix API
  slug: geocodio-distance-matrix-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geocodio/openapi/geocodio-distance-matrix-api-openapi.yml
- filename: geocodio-geocode-api-openapi.yml
  format: yaml
  label: Geocodio Geocode API
  slug: geocodio-geocode-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geocodio/openapi/geocodio-geocode-api-openapi.yml
- filename: geocodio-reverse-api-openapi.yml
  format: yaml
  label: Geocodio Reverse API
  slug: geocodio-reverse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/geocodio/openapi/geocodio-reverse-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Geocodio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geocodio secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Geocodio
provider_slug: geocodio
scheme_count: 1
schemes:
- description: Geocodio API key passed as the api_key query parameter.
  in: query
  name: apiKeyQuery
  parameter: api_key
  sources:
  - openapi/geocodio-openapi.yml
  type: apiKey
slug: geocodio-authentication
source_filename: geocodio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/geocodio-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Geocodio API key passed as the api_key query parameter.\n  sources:\n  - openapi/geocodio-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/geocodio/authentication/geocodio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Geocoding
- Reverse Geocoding
- Addresses
- Data Append
- Census
- Geospatial
---
