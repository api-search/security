---
api_key_in:
- query
api_specs:
- filename: symphony-pod-api-openapi.yml
  format: yaml
  label: Symphony Pod API
  slug: symphony-pod-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/symphony-pod-api-openapi.yml
- filename: agent-openapi-original.yml
  format: yaml
  label: Symphony Agent API
  slug: symphony-agent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/agent-openapi-original.yml
- filename: authenticator-openapi-original.yml
  format: yaml
  label: Symphony Authenticator API
  slug: symphony-authenticator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/authenticator-openapi-original.yml
- filename: login-openapi-original.yml
  format: yaml
  label: Symphony Login API
  slug: symphony-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/login-openapi-original.yml
- filename: profile-manager-openapi-original.yml
  format: yaml
  label: Symphony Profile Manager API
  slug: symphony-profile-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/profile-manager-openapi-original.yml
- filename: community-connect-openapi-original.yml
  format: yaml
  label: Symphony Community Connect API
  slug: symphony-community-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/openapi/community-connect-openapi-original.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Symphony Authentication
name_suffix: Authentication
oauth_flows: []
overview: Symphony secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Symphony
provider_slug: symphony
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: ExtApp JWT
  name: JwtAuth
  scheme: bearer
  sources:
  - openapi/community-connect-openapi-original.yml
  - openapi/pod-openapi-original.yml
  - openapi/profile-manager-openapi-original.yml
  - openapi/symphony-community-connect-api-openapi.yml
  type: http
- in: query
  name: ApiKeyAuth
  parameter: token
  sources:
  - openapi/community-connect-openapi-original.yml
  - openapi/symphony-community-connect-api-openapi.yml
  type: apiKey
slug: symphony-authentication
source_filename: symphony-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/community-connect-openapi-original.yml, openapi/pod-openapi-original.yml, openapi/profile-manager-openapi-original.yml,\n  openapi/symphony-community-connect-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: JwtAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: ExtApp JWT\n  sources:\n  - openapi/community-connect-openapi-original.yml\n  - openapi/pod-openapi-original.yml\n  - openapi/profile-manager-openapi-original.yml\n  - openapi/symphony-community-connect-api-openapi.yml\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: token\n  sources:\n  - openapi/community-connect-openapi-original.yml\n  - openapi/symphony-community-connect-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/symphony/refs/heads/main/authentication/symphony-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Collaboration
- Communication
- Financial Services
- Messaging
- Secure Communication
---
