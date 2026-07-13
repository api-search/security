---
api_key_in:
- header
api_specs:
- filename: swaggerhub-registry-api-openapi.yml
  format: yaml
  label: SwaggerHub Registry API
  slug: swaggerhub-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-registry-api-openapi.yml
- filename: swaggerhub-user-management-openapi.yml
  format: yaml
  label: SwaggerHub User Management API
  slug: swaggerhub-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/openapi/swaggerhub-user-management-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Swaggerhub Authentication
name_suffix: Authentication
oauth_flows: []
overview: SwaggerHub secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SwaggerHub
provider_slug: swaggerhub
scheme_count: 1
schemes:
- description: SwaggerHub API key. Obtain from My Account > API Key in SwaggerHub. Pass the key as the Authorization header value without any prefix.
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/swaggerhub-registry-api-openapi.yml
  - openapi/swaggerhub-user-management-openapi.yml
  type: apiKey
slug: swaggerhub-authentication
source_filename: swaggerhub-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/swaggerhub-registry-api-openapi.yml, openapi/swaggerhub-user-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: SwaggerHub API key. Obtain from My Account > API Key in SwaggerHub. Pass the\n    key as the Authorization header value without any prefix.\n  sources:\n  - openapi/swaggerhub-registry-api-openapi.yml\n  - openapi/swaggerhub-user-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swaggerhub/refs/heads/main/authentication/swaggerhub-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Design
- API Management
- API Registry
- Documentation
- OpenAPI
- SmartBear
---
