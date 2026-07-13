---
api_key_in:
- header
api_specs:
- filename: ngrok-api-openapi.yml
  format: yaml
  label: ngrok API
  slug: ngrok
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/openapi/ngrok-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ngrok Authentication
name_suffix: Authentication
oauth_flows: []
overview: ngrok secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ngrok
provider_slug: ngrok
scheme_count: 2
schemes:
- description: Use an ngrok API key as a Bearer token. Create API keys from the ngrok dashboard or via the API Keys endpoints.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/ngrok-api-openapi.yml
  type: http
- description: Pass the API key in the Authorization header prefixed with 'Bearer '.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/ngrok-api-openapi.yml
  type: apiKey
slug: ngrok-authentication
source_filename: ngrok-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ngrok-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Use an ngrok API key as a Bearer token. Create API keys from the ngrok dashboard\n    or via the API Keys endpoints.\n  sources:\n  - openapi/ngrok-api-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Pass the API key in the Authorization header prefixed with 'Bearer '.\n  sources:\n  - openapi/ngrok-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ngrok/refs/heads/main/authentication/ngrok-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- AI Gateway
- API Gateway
- Compute
- Developer Tools
- Gateways
- Ingress
- Platform
- Proxies
- Servers
- Tunnels
---
