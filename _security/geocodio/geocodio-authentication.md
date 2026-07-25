---
api_key_in:
- query
api_specs:
- filename: geocodio-batch-api-openapi.yml
  format: yaml
  label: Geocodio Batch API
  slug: geocodio-batch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-batch-api-openapi.yml
- filename: geocodio-forward-geocoding-api-openapi.yml
  format: yaml
  label: Geocodio Forward Geocoding API
  slug: geocodio-forward-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-forward-geocoding-api-openapi.yml
- filename: geocodio-lists-api-openapi.yml
  format: yaml
  label: Geocodio Lists API
  slug: geocodio-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-lists-api-openapi.yml
- filename: geocodio-reverse-geocoding-api-openapi.yml
  format: yaml
  label: Geocodio Reverse Geocoding API
  slug: geocodio-reverse-geocoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-reverse-geocoding-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/authentication/geocodio-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Geocoding
- Reverse Geocoding
- Addresses
- Data Append
- Census
---
