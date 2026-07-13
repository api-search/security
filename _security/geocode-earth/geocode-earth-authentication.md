---
api_key_in:
- query
api_specs:
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Search API
  slug: search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Autocomplete API
  slug: autocomplete
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Reverse API
  slug: reverse
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Structured Search API
  slug: structured-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
- filename: geocode-earth-openapi.yml
  format: yaml
  label: Geocode Earth Place API
  slug: place
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/openapi/geocode-earth-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Geocode Earth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Geocode Earth secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Geocode Earth
provider_slug: geocode-earth
scheme_count: 1
schemes:
- description: Geocode Earth API key passed as the api_key query string parameter.
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/geocode-earth-openapi.yml
  type: apiKey
slug: geocode-earth-authentication
source_filename: geocode-earth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/geocode-earth-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Geocode Earth API key passed as the api_key query string parameter.\n  sources:\n  - openapi/geocode-earth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocode-earth/refs/heads/main/authentication/geocode-earth-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Geocoding
- Address Autocomplete
- Reverse Geocoding
- Mapping
- Pelias
- Open Data
---
