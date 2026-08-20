---
api_key_in:
- header
api_specs:
- filename: istock-countries-api-openapi.yml
  format: yaml
  label: iStock Countries API
  slug: istock-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istock/refs/heads/main/openapi/istock-countries-api-openapi.yml
- filename: istock-downloads-api-openapi.yml
  format: yaml
  label: iStock Downloads API
  slug: istock-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istock/refs/heads/main/openapi/istock-downloads-api-openapi.yml
- filename: istock-images-api-openapi.yml
  format: yaml
  label: iStock Images API
  slug: istock-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istock/refs/heads/main/openapi/istock-images-api-openapi.yml
- filename: istock-oauth-api-openapi.yml
  format: yaml
  label: iStock OAuth API
  slug: istock-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istock/refs/heads/main/openapi/istock-oauth-api-openapi.yml
- filename: istock-search-api-openapi.yml
  format: yaml
  label: iStock Search API
  slug: istock-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istock/refs/heads/main/openapi/istock-search-api-openapi.yml
- filename: istock-videos-api-openapi.yml
  format: yaml
  label: iStock Videos API
  slug: istock-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/istock/refs/heads/main/openapi/istock-videos-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Istock Authentication
name_suffix: Authentication
oauth_flows: []
overview: iStock secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: iStock
provider_slug: istock
scheme_count: 2
schemes:
- description: API key issued through the Getty Images developer program.
  in: header
  name: apiKey
  parameter: api-key
  sources:
  - openapi/istock-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: OAuth 2.0 access token obtained via /oauth2/token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/istock-openapi.yml
  type: http
slug: istock-authentication
source_filename: istock-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/istock-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: API key issued through the Getty Images developer program.\n  sources:\n  - openapi/istock-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth 2.0 access token obtained via /oauth2/token.\n  sources:\n  - openapi/istock-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/istock/refs/heads/main/authentication/istock-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Stock Media
- Image
- Video
- Illustrations
- Royalty-Free
- Getty
---
