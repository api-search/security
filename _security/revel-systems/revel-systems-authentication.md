---
api_key_in:
- header
api_specs:
- filename: revel-open-api-openapi.yml
  format: yaml
  label: Revel Open API
  slug: open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revel-systems/refs/heads/main/openapi/revel-open-api-openapi.yml
- filename: revel-webhooks-asyncapi.yml
  format: yaml
  label: Revel Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/revel-systems/refs/heads/main/asyncapi/revel-webhooks-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Revel Systems Authentication
name_suffix: Authentication
oauth_flows: []
overview: Revel Systems secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Revel Systems
provider_slug: revel-systems
scheme_count: 1
schemes:
- description: 'API key and secret joined by a colon, e.g. `API-AUTHENTICATION: key:secret`. The key and secret may alternatively be passed as `api_key` and `api_secret` query parameters.'
  in: header
  name: apiAuthentication
  parameter: API-AUTHENTICATION
  sources:
  - openapi/revel-open-api-openapi.yml
  type: apiKey
slug: revel-systems-authentication
source_filename: revel-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/revel-open-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiAuthentication\n  type: apiKey\n  in: header\n  parameter: API-AUTHENTICATION\n  description: 'API key and secret joined by a colon, e.g. `API-AUTHENTICATION: key:secret`.\n    The key and secret may alternatively be passed as `api_key` and `api_secret` query parameters.'\n  sources:\n  - openapi/revel-open-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revel-systems/refs/heads/main/authentication/revel-systems-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- POS
- Restaurant
- Retail
- iPad
---
