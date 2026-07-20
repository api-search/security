---
api_key_in:
- header
api_specs:
- filename: indykite-rest-openapi.yml
  format: yaml
  label: IndyKite REST API
  slug: indykite-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indykite/refs/heads/main/openapi/indykite-rest-openapi.yml
- filename: indykite-config-openapi.yml
  format: yaml
  label: IndyKite Config REST API
  slug: indykite-config-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/indykite/refs/heads/main/openapi/indykite-config-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Indykite Authentication
name_suffix: Authentication
oauth_flows: []
overview: Indykite secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Indykite
provider_slug: indykite
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Bearer token generated from Service Account credentials.
  name: BearerToken
  scheme: bearer
  sources:
  - openapi/indykite-config-openapi.yml
  - openapi/indykite-rest-openapi.yml
  type: http
- description: The value of the App Agent credential header must be passed as is, without any prefix.
  in: header
  name: APIKey
  parameter: X-IK-ClientKey
  sources:
  - openapi/indykite-rest-openapi.yml
  type: apiKey
slug: indykite-authentication
source_filename: indykite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/indykite-config-openapi.yml, openapi/indykite-rest-openapi.yml\ndocs: https://docs.indykite.com/docs/apis/sdks\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token generated from Service Account credentials.\n  sources:\n  - openapi/indykite-config-openapi.yml\n  - openapi/indykite-rest-openapi.yml\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: X-IK-ClientKey\n  description: The value of the App Agent credential header must be passed as is, without any\n    prefix.\n  sources:\n  - openapi/indykite-rest-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/indykite/refs/heads/main/authentication/indykite-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Identity
- Authorization
- Access Control
- Knowledge Graph
- Agentic AI
- MCP
- Security
- AuthZEN
---
