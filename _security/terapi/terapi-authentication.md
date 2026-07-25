---
api_key_in:
- header
api_specs:
- filename: terapi-actions-api-openapi.yml
  format: yaml
  label: Terapi Actions API
  slug: terapi-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terapi/refs/heads/main/openapi/terapi-actions-api-openapi.yml
- filename: terapi-authentication-api-openapi.yml
  format: yaml
  label: Terapi Authentication API
  slug: terapi-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terapi/refs/heads/main/openapi/terapi-authentication-api-openapi.yml
- filename: terapi-connections-api-openapi.yml
  format: yaml
  label: Terapi Connections API
  slug: terapi-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terapi/refs/heads/main/openapi/terapi-connections-api-openapi.yml
- filename: terapi-integrations-api-openapi.yml
  format: yaml
  label: Terapi Integrations API
  slug: terapi-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terapi/refs/heads/main/openapi/terapi-integrations-api-openapi.yml
- filename: terapi-sync-api-openapi.yml
  format: yaml
  label: Terapi Sync API
  slug: terapi-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/terapi/refs/heads/main/openapi/terapi-sync-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Terapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Terapi secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Terapi
provider_slug: terapi
scheme_count: 1
schemes:
- description: Secret key from Terapi environment settings. Passed as 'Bearer {secret_key}'
  in: header
  name: SecretKeyAuth
  parameter: Authorization
  sources:
  - openapi/terapi-openapi.yml
  type: apiKey
slug: terapi-authentication
source_filename: terapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/terapi-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SecretKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Secret key from Terapi environment settings. Passed as 'Bearer {secret_key}'\n  sources:\n  - openapi/terapi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/terapi/refs/heads/main/authentication/terapi-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Authentication
- Connectors
- Embedded iPaaS
- Integration
- Native Integrations
- Open Source
- Workflow Automation
---
