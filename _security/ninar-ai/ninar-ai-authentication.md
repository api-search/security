---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ninar-ai-crm-api-openapi.yml
  format: yaml
  label: Ninar AI CRM API
  slug: ninar-ai-crm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ninar-ai/openapi/ninar-ai-crm-api-openapi.yml
- filename: ninar-ai-visibility-api-openapi.yml
  format: yaml
  label: Ninar AI Visibility API
  slug: ninar-ai-visibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ninar-ai/openapi/ninar-ai-visibility-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Ninar AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ninar AI secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ninar AI
provider_slug: ninar-ai
scheme_count: 2
schemes:
- in: header
  name: crmApiKey
  parameter: X-API-Key
  sources:
  - openapi/ninar-ai-openapi.yml
  type: apiKey
- name: visibilityBearer
  scheme: bearer
  sources:
  - openapi/ninar-ai-openapi.yml
  type: http
slug: ninar-ai-authentication
source_filename: ninar-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/ninar-ai-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: crmApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/ninar-ai-openapi.yml\n- name: visibilityBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/ninar-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/ninar-ai/authentication/ninar-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Marketing
- Analytics
- Brand Visibility
- Software-as-a-Service
---
