---
api_key_in:
- cookie
api_specs:
- filename: gravitee-apim-openapi.yml
  format: yaml
  label: Gravitee API Management
  slug: gravitee-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gravitee/refs/heads/main/openapi/gravitee-apim-openapi.yml
- filename: gravitee-am-openapi.yml
  format: yaml
  label: Gravitee Access Management
  slug: gravitee-access-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gravitee/refs/heads/main/openapi/gravitee-am-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gravitee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gravitee secures its APIs with apiKey and http across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gravitee
provider_slug: gravitee
scheme_count: 4
schemes:
- name: gravitee-auth
  scheme: Bearer
  sources:
  - openapi/gravitee-am-openapi.yml
  type: http
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/gravitee-apim-openapi.yml
  type: http
- in: cookie
  name: CookieAuth
  parameter: Auth-Graviteeio-APIM
  sources:
  - openapi/gravitee-apim-openapi.yml
  type: apiKey
- bearerFormat: JWT
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/gravitee-apim-openapi.yml
  type: http
slug: gravitee-authentication
source_filename: gravitee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gravitee-am-openapi.yml, openapi/gravitee-apim-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: gravitee-auth\n  type: http\n  scheme: Bearer\n  sources:\n  - openapi/gravitee-am-openapi.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/gravitee-apim-openapi.yml\n- name: CookieAuth\n  type: apiKey\n  in: cookie\n  parameter: Auth-Graviteeio-APIM\n  sources:\n  - openapi/gravitee-apim-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/gravitee-apim-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gravitee/refs/heads/main/authentication/gravitee-authentication.yml
summary_line: apiKey/http · 4 schemes
tags:
- API Gateway
- API Management
- Access Management
- Identity
- Event-Driven
- Event Management
- Kafka Gateway
- Kafka
- MQTT
- GraphQL
- gRPC
- AI Gateway
- MCP
- A2A
- LLM Proxy
- Multi-Gateway Federation
- Developer Portal
- Open Source
- Apache 2.0
---
