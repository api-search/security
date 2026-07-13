---
api_key_in:
- header
api_specs:
- filename: seamless-ai-contacts-openapi.yml
  format: yaml
  label: Seamless.AI Contacts API
  slug: seamless-ai-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/openapi/seamless-ai-contacts-openapi.yml
- filename: seamless-ai-companies-openapi.yml
  format: yaml
  label: Seamless.AI Companies API
  slug: seamless-ai-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/openapi/seamless-ai-companies-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Seamless Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seamless.AI secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Seamless.AI
provider_slug: seamless-ai
scheme_count: 1
schemes:
- description: API key in the format "Bearer {api_key}"
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/seamless-ai-companies-openapi.yml
  - openapi/seamless-ai-contacts-openapi.yml
  type: apiKey
slug: seamless-ai-authentication
source_filename: seamless-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/seamless-ai-companies-openapi.yml, openapi/seamless-ai-contacts-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key in the format \"Bearer {api_key}\"\n  sources:\n  - openapi/seamless-ai-companies-openapi.yml\n  - openapi/seamless-ai-contacts-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seamless-ai/refs/heads/main/authentication/seamless-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- B2B
- Contact Data
- Sales Intelligence
- Prospecting
- Lead Generation
- CRM Enrichment
---
