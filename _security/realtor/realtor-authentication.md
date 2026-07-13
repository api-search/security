---
api_key_in:
- header
api_specs:
- filename: realtor-connections-plus-asyncapi.yml
  format: yaml
  label: Realtor.com Connections Plus API
  slug: connections-plus-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/asyncapi/realtor-connections-plus-asyncapi.yml
- filename: realtor-lead-delivery-asyncapi.yml
  format: yaml
  label: Realtor.com Lead Delivery API
  slug: lead-delivery-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/asyncapi/realtor-lead-delivery-asyncapi.yml
- filename: realtor-property-data-openapi.yml
  format: yaml
  label: Realtor.com Property Data API
  slug: property-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/openapi/realtor-property-data-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Realtor Authentication
name_suffix: Authentication
oauth_flows: []
overview: realtor secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: realtor
provider_slug: realtor
scheme_count: 1
schemes:
- description: API key provided by RapidAPI for authenticating requests.
  in: header
  name: rapidApiKey
  parameter: X-RapidAPI-Key
  sources:
  - openapi/realtor-property-data-openapi.yml
  type: apiKey
slug: realtor-authentication
source_filename: realtor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/realtor-property-data-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: rapidApiKey\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  description: API key provided by RapidAPI for authenticating requests.\n  sources:\n  - openapi/realtor-property-data-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/realtor/refs/heads/main/authentication/realtor-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
