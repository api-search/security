---
api_key_in:
- header
api_specs:
- filename: kaedim-assets-api-openapi.yml
  format: yaml
  label: Kaedim Assets API
  slug: kaedim-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaedim/refs/heads/main/openapi/kaedim-assets-api-openapi.yml
- filename: kaedim-auth-api-openapi.yml
  format: yaml
  label: Kaedim Auth API
  slug: kaedim-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaedim/refs/heads/main/openapi/kaedim-auth-api-openapi.yml
- filename: kaedim-generation-api-openapi.yml
  format: yaml
  label: Kaedim Generation API
  slug: kaedim-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaedim/refs/heads/main/openapi/kaedim-generation-api-openapi.yml
- filename: kaedim-webhooks-api-openapi.yml
  format: yaml
  label: Kaedim Webhooks API
  slug: kaedim-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kaedim/refs/heads/main/openapi/kaedim-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Kaedim Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kaedim secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Kaedim
provider_slug: kaedim
scheme_count: 2
schemes:
- description: Enterprise API key from Settings > API Keys in the Kaedim app.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/kaedim-web-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: JWT obtained via /registerHook, refreshed via /refreshJWT every 12 hours.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/kaedim-web-api-openapi.yml
  type: http
slug: kaedim-authentication
source_filename: kaedim-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kaedim-web-api-openapi.yml\ndocs: https://docs.kaedim3d.com/enterprise-features/custom-integrations/apis/web-api\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Enterprise API key from Settings > API Keys in the Kaedim app.\n  sources:\n  - openapi/kaedim-web-api-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT obtained via /registerHook, refreshed via /refreshJWT every 12 hours.\n  sources:\n  - openapi/kaedim-web-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kaedim/refs/heads/main/authentication/kaedim-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- 3D
- Artificial Intelligence
- Generative AI
- Gaming
- 3D Models
- Asset Generation
- Content Generation
- Machine-Learning
---
