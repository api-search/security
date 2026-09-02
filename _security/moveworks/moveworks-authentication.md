---
api_key_in:
- header
api_specs:
- filename: moveworks-authentication-api-openapi.yml
  format: yaml
  label: Moveworks authentication API
  slug: moveworks-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-authentication-api-openapi.yml
- filename: moveworks-conversations-api-openapi.yml
  format: yaml
  label: Moveworks conversations API
  slug: moveworks-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-conversations-api-openapi.yml
- filename: moveworks-default-api-openapi.yml
  format: yaml
  label: Moveworks Default API
  slug: moveworks-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-default-api-openapi.yml
- filename: moveworks-deprecated-api-openapi.yml
  format: yaml
  label: Moveworks deprecated API
  slug: moveworks-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-deprecated-api-openapi.yml
- filename: moveworks-events-api-openapi.yml
  format: yaml
  label: Moveworks events API
  slug: moveworks-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-events-api-openapi.yml
- filename: moveworks-messages-api-openapi.yml
  format: yaml
  label: Moveworks messages API
  slug: moveworks-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-messages-api-openapi.yml
- filename: moveworks-responses-api-openapi.yml
  format: yaml
  label: Moveworks responses API
  slug: moveworks-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-responses-api-openapi.yml
- filename: moveworks-smartforms-api-openapi.yml
  format: yaml
  label: Moveworks smartForms API
  slug: moveworks-smartforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-smartforms-api-openapi.yml
- filename: moveworks-webhooks-api-openapi.yml
  format: yaml
  label: Moveworks webhooks API
  slug: moveworks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/openapi/moveworks-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Moveworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moveworks secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Moveworks
provider_slug: moveworks
scheme_count: 3
schemes:
- description: JWT bearer token authentication. Obtain an access token from the Moveworks auth endpoint and include it in the Authorization header as 'Bearer <token>'.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/moveworks-beta-conversations-api-openapi.yaml
  - openapi/moveworks-conversations-api-openapi.yaml
  - openapi/moveworks-data-api-openapi.yaml
  - openapi/moveworks-events-api-openapi.yaml
  - openapi/moveworks-forms-gateway-openapi.yaml
  - openapi/moveworks-identity-gateway-openapi.yaml
  - openapi/moveworks-knowledge-gateway-openapi.yaml
  - openapi/moveworks-webhook-listeners-openapi.yaml
  type: http
- in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/moveworks-data-api-openapi.yaml
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/moveworks-forms-gateway-openapi.yaml
  type: apiKey
slug: moveworks-authentication
source_filename: moveworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/moveworks-beta-conversations-api-openapi.yaml, openapi/moveworks-conversations-api-openapi.yaml,\n  openapi/moveworks-data-api-openapi.yaml, openapi/moveworks-events-api-openapi.yaml, openapi/moveworks-forms-gateway-openapi.yaml,\n  openapi/moveworks-identity-gateway-openapi.yaml, openapi/moveworks-knowledge-gateway-openapi.yaml,\n  openapi/moveworks-webhook-listeners-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: JWT bearer token authentication. Obtain an access token from the Moveworks auth\n    endpoint and include it in the Authorization header as 'Bearer <token>'.\n  sources:\n  - openapi/moveworks-beta-conversations-api-openapi.yaml\n  - openapi/moveworks-conversations-api-openapi.yaml\n  - openapi/moveworks-data-api-openapi.yaml\n  - openapi/moveworks-events-api-openapi.yaml\n  - openapi/moveworks-forms-gateway-openapi.yaml\n\
  \  - openapi/moveworks-identity-gateway-openapi.yaml\n  - openapi/moveworks-knowledge-gateway-openapi.yaml\n  - openapi/moveworks-webhook-listeners-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/moveworks-data-api-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/moveworks-forms-gateway-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moveworks/refs/heads/main/authentication/moveworks-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Artificial Intelligence
- Agentic AI
- AI Assistant
- Enterprise Automation
- Conversational AI
- Employee Experience
- ITSM
- Enterprise Search
---
