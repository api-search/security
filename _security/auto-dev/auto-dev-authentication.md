---
api_key_in:
- query
api_specs:
- filename: auto-dev-dealers-api-openapi.yml
  format: yaml
  label: Auto.dev Dealers API
  slug: auto-dev-dealers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-dealers-api-openapi.yml
- filename: auto-dev-listings-api-openapi.yml
  format: yaml
  label: Auto.dev Listings API
  slug: auto-dev-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-listings-api-openapi.yml
- filename: auto-dev-market-value-api-openapi.yml
  format: yaml
  label: Auto.dev Market Value API
  slug: auto-dev-market-value-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-market-value-api-openapi.yml
- filename: auto-dev-recalls-api-openapi.yml
  format: yaml
  label: Auto.dev Recalls API
  slug: auto-dev-recalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-recalls-api-openapi.yml
- filename: auto-dev-vin-decoding-api-openapi.yml
  format: yaml
  label: Auto.dev VIN Decoding API
  slug: auto-dev-vin-decoding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/openapi/auto-dev-vin-decoding-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Auto Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Auto.dev secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Auto.dev
provider_slug: auto-dev
scheme_count: 2
schemes:
- description: Supply your Auto.dev API key as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/auto-dev-openapi.yml
  type: http
- description: Supply your Auto.dev API key as the apikey query parameter.
  in: query
  name: apiKeyQuery
  parameter: apikey
  sources:
  - openapi/auto-dev-openapi.yml
  type: apiKey
slug: auto-dev-authentication
source_filename: auto-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/auto-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Supply your Auto.dev API key as a Bearer token.\n  sources:\n  - openapi/auto-dev-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  description: Supply your Auto.dev API key as the apikey query parameter.\n  sources:\n  - openapi/auto-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auto-dev/refs/heads/main/authentication/auto-dev-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Automotive
- Vehicle Data
- VIN Decoding
- Vehicle Listings
- Recalls
---
