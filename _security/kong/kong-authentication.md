---
api_key_in:
- header
api_specs:
- filename: kong-gateway-admin-api.yml
  format: yaml
  label: Kong Gateway Admin API
  slug: kong-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/openapi/kong-gateway-admin-api.yml
- filename: kong-konnect-platform-api.yml
  format: yaml
  label: Kong Konnect Platform API
  slug: kong-konnect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/openapi/kong-konnect-platform-api.yml
- filename: openapi.yaml
  format: yaml
  label: Kong Event Gateway
  slug: kong-event-gateway
  spec_type: OpenAPI
  url: https://developer.konghq.com/api/konnect/event-gateway/v1/
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kong Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kong secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kong
provider_slug: kong
scheme_count: 2
schemes:
- in: header
  name: adminToken
  parameter: Kong-Admin-Token
  sources:
  - openapi/kong-gateway-admin-api.yml
  type: apiKey
- bearerFormat: Token
  description: The personal access token is meant to be used as an alternative to basic-auth when accessing Konnect via APIs. You can generate a Personal Access Token (PAT) from the personal access token page in the Konnect dashboard.
  name: personalAccessToken
  scheme: bearer
  sources:
  - openapi/kong-konnect-platform-api.yml
  type: http
slug: kong-authentication
source_filename: kong-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kong-gateway-admin-api.yml, openapi/kong-konnect-platform-api.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: adminToken\n  type: apiKey\n  in: header\n  parameter: Kong-Admin-Token\n  sources:\n  - openapi/kong-gateway-admin-api.yml\n- name: personalAccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: Token\n  description: The personal access token is meant to be used as an alternative to basic-auth\n    when accessing Konnect via APIs. You can generate a Personal Access Token (PAT) from the\n    personal access token page in the Konnect dashboard.\n  sources:\n  - openapi/kong-konnect-platform-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kong/refs/heads/main/authentication/kong-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- API Gateway
- AI Gateway
- AI Connectivity
- Agent Gateway
- Event Gateway
- MCP Registry
- Service Mesh
- LLM
- Kafka
- Konnect
- Open Source
---
