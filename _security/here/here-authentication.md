---
api_key_in:
- query
api_specs:
- filename: here-autocomplete-api-openapi.yml
  format: yaml
  label: HERE Autocomplete API
  slug: here-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here/refs/heads/main/openapi/here-autocomplete-api-openapi.yml
- filename: here-autosuggest-api-openapi.yml
  format: yaml
  label: HERE Autosuggest API
  slug: here-autosuggest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here/refs/heads/main/openapi/here-autosuggest-api-openapi.yml
- filename: here-browse-api-openapi.yml
  format: yaml
  label: HERE Browse API
  slug: here-browse-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here/refs/heads/main/openapi/here-browse-api-openapi.yml
- filename: here-discover-api-openapi.yml
  format: yaml
  label: HERE Discover API
  slug: here-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here/refs/heads/main/openapi/here-discover-api-openapi.yml
- filename: here-geocode-api-openapi.yml
  format: yaml
  label: HERE Geocode API
  slug: here-geocode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here/refs/heads/main/openapi/here-geocode-api-openapi.yml
- filename: here-lookup-api-openapi.yml
  format: yaml
  label: HERE Lookup API
  slug: here-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here/refs/heads/main/openapi/here-lookup-api-openapi.yml
- filename: here-reverse-geocode-api-openapi.yml
  format: yaml
  label: HERE Reverse Geocode API
  slug: here-reverse-geocode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/here/refs/heads/main/openapi/here-reverse-geocode-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Here Authentication
name_suffix: Authentication
oauth_flows: []
overview: HERE secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: HERE
provider_slug: here
scheme_count: 2
schemes:
- description: HERE API Key (apiKey query parameter)
  in: query
  name: apiKey
  parameter: apiKey
  sources:
  - openapi/here-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: HERE OAuth 2.0 token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/here-openapi.yml
  type: http
slug: here-authentication
source_filename: here-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/here-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: apiKey\n  description: HERE API Key (apiKey query parameter)\n  sources:\n  - openapi/here-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: HERE OAuth 2.0 token\n  sources:\n  - openapi/here-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/here/refs/heads/main/authentication/here-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Location
- Mapping
- Maps
- Spatial
---
