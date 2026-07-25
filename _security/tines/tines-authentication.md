---
api_key_in:
- header
api_specs:
- filename: tines-actions-api-openapi.yml
  format: yaml
  label: Tines Actions API
  slug: tines-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-actions-api-openapi.yml
- filename: tines-audit-logs-api-openapi.yml
  format: yaml
  label: Tines Audit Logs API
  slug: tines-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-audit-logs-api-openapi.yml
- filename: tines-credentials-api-openapi.yml
  format: yaml
  label: Tines Credentials API
  slug: tines-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-credentials-api-openapi.yml
- filename: tines-folders-api-openapi.yml
  format: yaml
  label: Tines Folders API
  slug: tines-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-folders-api-openapi.yml
- filename: tines-stories-api-openapi.yml
  format: yaml
  label: Tines Stories API
  slug: tines-stories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-stories-api-openapi.yml
- filename: tines-tags-api-openapi.yml
  format: yaml
  label: Tines Tags API
  slug: tines-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-tags-api-openapi.yml
- filename: tines-teams-api-openapi.yml
  format: yaml
  label: Tines Teams API
  slug: tines-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/openapi/tines-teams-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Tines Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tines secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tines
provider_slug: tines
scheme_count: 2
schemes:
- description: 'Bearer token authentication using an Tines API key. Format: `Authorization: Bearer <api_key>`'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tines-rest-api-openapi.yml
  type: http
- description: 'API key authentication using the X-User-Token header. Format: `X-User-Token: <api_key>`'
  in: header
  name: ApiKeyAuth
  parameter: X-User-Token
  sources:
  - openapi/tines-rest-api-openapi.yml
  type: apiKey
slug: tines-authentication
source_filename: tines-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/tines-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token authentication using an Tines API key. Format: `Authorization:\n    Bearer <api_key>`'\n  sources:\n  - openapi/tines-rest-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-User-Token\n  description: 'API key authentication using the X-User-Token header. Format: `X-User-Token:\n    <api_key>`'\n  sources:\n  - openapi/tines-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tines/refs/heads/main/authentication/tines-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Security Automation
- No-Code
- Workflow Automation
- Security Operations
- SOAR
- Incident Response
- REST API
- Webhooks
---
