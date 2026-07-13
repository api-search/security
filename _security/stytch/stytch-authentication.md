---
api_key_in: []
api_specs:
- filename: stytch-consumer-openapi.yml
  format: yaml
  label: Stytch Consumer Authentication API
  slug: stytch-consumer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/openapi/stytch-consumer-openapi.yml
- filename: stytch-b2b-openapi.yml
  format: yaml
  label: Stytch B2B Authentication API
  slug: stytch-b2b-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/openapi/stytch-b2b-openapi.yml
- filename: stytch-management-openapi.yml
  format: yaml
  label: Stytch Management API
  slug: stytch-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/openapi/stytch-management-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stytch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stytch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stytch
provider_slug: stytch
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/stytch-b2b-openapi.yml
  - openapi/stytch-consumer-openapi.yml
  - openapi/stytch-management-openapi.yml
  type: http
slug: stytch-authentication
source_filename: stytch-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stytch-b2b-openapi.yml, openapi/stytch-consumer-openapi.yml, openapi/stytch-management-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/stytch-b2b-openapi.yml\n  - openapi/stytch-consumer-openapi.yml\n  - openapi/stytch-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stytch/refs/heads/main/authentication/stytch-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Identity
- Passwordless
- Security
- B2B
- Connected Apps
- MCP
- AI Agents
- Developer Tools
---
