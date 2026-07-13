---
api_key_in:
- header
api_specs:
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Admin Members API
  slug: circle-community-admin-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Admin Spaces API
  slug: circle-community-admin-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Admin Posts and Comments API
  slug: circle-community-admin-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Admin Events API
  slug: circle-community-admin-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Admin Courses API
  slug: circle-community-admin-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Headless Member API
  slug: circle-community-headless-member-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-openapi.yml
  format: yaml
  label: Circle Headless Auth API
  slug: circle-community-headless-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/openapi/circle-community-openapi.yml
- filename: circle-community-asyncapi.yml
  format: yaml
  label: Circle Realtime WebSocket API
  slug: circle-community-realtime-websocket-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/asyncapi/circle-community-asyncapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Circle Community Authentication
name_suffix: Authentication
oauth_flows: []
overview: Circle secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Circle
provider_slug: circle-community
scheme_count: 2
schemes:
- description: Admin API token in the format "Token AUTH_TOKEN". Community admins generate the token on the Developers -> Tokens page.
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/circle-community-openapi.yml
  type: apiKey
- description: Member-scoped JWT access token from /api/v1/headless/auth_token in the format "Bearer ACCESS_TOKEN". Expires after one hour.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/circle-community-openapi.yml
  type: http
slug: circle-community-authentication
source_filename: circle-community-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/circle-community-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Admin API token in the format \"Token AUTH_TOKEN\". Community admins generate the\n    token on the Developers -> Tokens page.\n  sources:\n  - openapi/circle-community-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Member-scoped JWT access token from /api/v1/headless/auth_token in the format\n    \"Bearer ACCESS_TOKEN\". Expires after one hour.\n  sources:\n  - openapi/circle-community-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/circle-community/refs/heads/main/authentication/circle-community-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Community
- Creators
- Courses
- Memberships
- Events
- Chat
- Community Platform
---
