---
api_key_in:
- header
api_specs:
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Authentication API
  slug: terra-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra User Management API
  slug: terra-api-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Activity API
  slug: terra-api-activity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Body API
  slug: terra-api-body-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Daily API
  slug: terra-api-daily-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Sleep API
  slug: terra-api-sleep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Nutrition API
  slug: terra-api-nutrition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Menstruation API
  slug: terra-api-menstruation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Athlete API
  slug: terra-api-athlete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
- filename: terra-api-openapi.yml
  format: yaml
  label: Terra Integrations API
  slug: terra-api-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/openapi/terra-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Terra Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terra secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Terra
provider_slug: terra-api
scheme_count: 2
schemes:
- description: Your public Terra developer identifier.
  in: header
  name: devId
  parameter: dev-id
  sources:
  - openapi/terra-api-openapi.yml
  type: apiKey
- description: Your secret Terra API key.
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/terra-api-openapi.yml
  type: apiKey
slug: terra-api-authentication
source_filename: terra-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/terra-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: devId\n  type: apiKey\n  in: header\n  parameter: dev-id\n  description: Your public Terra developer identifier.\n  sources:\n  - openapi/terra-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Your secret Terra API key.\n  sources:\n  - openapi/terra-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terra-api/refs/heads/main/authentication/terra-api-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Wearables
- Health Data
- Fitness
- Aggregator
- Webhooks
- Digital Health
---
