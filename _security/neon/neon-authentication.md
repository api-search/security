---
api_key_in: []
api_specs:
- filename: neon-management-api-openapi.yml
  format: yaml
  label: Neon Management API
  slug: management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/openapi/neon-management-api-openapi.yml
- filename: neon-auth-webhooks-asyncapi.yml
  format: yaml
  label: Neon Auth
  slug: auth
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/asyncapi/neon-auth-webhooks-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Neon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Neon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Neon
provider_slug: neon
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: Neon API keys are used to authenticate requests. Include the API key in the Authorization header as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/neon-management-api-openapi.yml
  type: http
slug: neon-authentication
source_filename: neon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/neon-management-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: Neon API keys are used to authenticate requests. Include the API key in the Authorization\n    header as a Bearer token.\n  sources:\n  - openapi/neon-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neon/refs/heads/main/authentication/neon-authentication.yml
summary_line: http · 1 scheme
tags:
- Databases
- Serverless
- Postgres
- Infrastructure
- Authentication
- Edge
---
