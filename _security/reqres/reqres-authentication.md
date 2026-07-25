---
api_key_in:
- header
api_specs:
- filename: reqres-agent-sandbox-api-openapi.yml
  format: yaml
  label: ReqRes Agent Sandbox API
  slug: reqres-agent-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reqres/refs/heads/main/openapi/reqres-agent-sandbox-api-openapi.yml
- filename: reqres-app-users-api-openapi.yml
  format: yaml
  label: ReqRes App Users API
  slug: reqres-app-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reqres/refs/heads/main/openapi/reqres-app-users-api-openapi.yml
- filename: reqres-authentication-api-openapi.yml
  format: yaml
  label: ReqRes Authentication API
  slug: reqres-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reqres/refs/heads/main/openapi/reqres-authentication-api-openapi.yml
- filename: reqres-collections-api-openapi.yml
  format: yaml
  label: ReqRes Collections API
  slug: reqres-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reqres/refs/heads/main/openapi/reqres-collections-api-openapi.yml
- filename: reqres-custom-endpoints-api-openapi.yml
  format: yaml
  label: ReqRes Custom Endpoints API
  slug: reqres-custom-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reqres/refs/heads/main/openapi/reqres-custom-endpoints-api-openapi.yml
- filename: reqres-legacy-api-openapi.yml
  format: yaml
  label: ReqRes Legacy API
  slug: reqres-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/reqres/refs/heads/main/openapi/reqres-legacy-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Reqres Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReqRes secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ReqRes
provider_slug: reqres
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/reqres-openapi.yml
  type: apiKey
- bearerFormat: session_token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/reqres-openapi.yml
  type: http
slug: reqres-authentication
source_filename: reqres-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/reqres-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/reqres-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: session_token\n  sources:\n  - openapi/reqres-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reqres/refs/heads/main/authentication/reqres-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Development
- Testing
- Prototyping
- Fake API
- REST
- Agent Sandbox
---
