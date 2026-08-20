---
api_key_in:
- header
api_specs:
- filename: apipark-ai-models-api-openapi.yml
  format: yaml
  label: APIPark AI Models API
  slug: apipark-ai-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apipark/refs/heads/main/openapi/apipark-ai-models-api-openapi.yml
- filename: apipark-services-api-openapi.yml
  format: yaml
  label: APIPark Services API
  slug: apipark-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apipark/refs/heads/main/openapi/apipark-services-api-openapi.yml
- filename: apipark-subscriptions-api-openapi.yml
  format: yaml
  label: APIPark Subscriptions API
  slug: apipark-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apipark/refs/heads/main/openapi/apipark-subscriptions-api-openapi.yml
- filename: apipark-teams-api-openapi.yml
  format: yaml
  label: APIPark Teams API
  slug: apipark-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apipark/refs/heads/main/openapi/apipark-teams-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apipark Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIPark secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIPark
provider_slug: apipark
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/apipark-api.yaml
  type: apiKey
slug: apipark-authentication
source_filename: apipark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apipark-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/apipark-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apipark/refs/heads/main/authentication/apipark-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Gateway
- API Gateway
- API Management
- Developer Portal
- LLM
- Open-Source
---
