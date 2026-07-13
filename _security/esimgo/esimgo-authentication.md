---
api_key_in:
- header
api_specs:
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Catalogue API
  slug: catalogue
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Orders API
  slug: orders
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go eSIMs API
  slug: esims
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Inventory API
  slug: inventory
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Network API
  slug: network
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
- filename: esimgo-openapi.yml
  format: yaml
  label: eSIM Go Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/openapi/esimgo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Esimgo Authentication
name_suffix: Authentication
oauth_flows: []
overview: eSIM Go secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: eSIM Go
provider_slug: esimgo
scheme_count: 1
schemes:
- description: Organisation API key. Find it under Account Settings -> API Details in your eSIM Go account and send it in the X-API-Key request header.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/esimgo-openapi.yml
  type: apiKey
slug: esimgo-authentication
source_filename: esimgo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/esimgo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Organisation API key. Find it under Account Settings -> API Details in your eSIM\n    Go account and send it in the X-API-Key request header.\n  sources:\n  - openapi/esimgo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/esimgo/refs/heads/main/authentication/esimgo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- eSIM
- Connectivity
- Travel Data
- Telecom
- Mobile
---
