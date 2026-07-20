---
api_key_in:
- header
- query
api_specs:
- filename: bucket-management-openapi-original.json
  format: json
  label: Reflag Management API
  slug: reflag-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bucket/refs/heads/main/openapi/bucket-management-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Bucket Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bucket secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bucket
provider_slug: bucket
scheme_count: 1
schemes:
- description: API key authentication, for service access (Management API)
  name: APIKey
  scheme: bearer
  sources:
  - openapi/bucket-management-openapi-original.json
  type: http
slug: bucket-authentication
source_filename: bucket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.reflag.com/api/api-access + openapi/bucket-management-openapi-original.json\ndocs: https://docs.reflag.com/api/api-access\nsummary:\n  types:\n  - http\n  api_key_in:\n  - header\n  - query\n  oauth2_flows: []\n  note: >-\n    Bearer-token (API-key) auth across both APIs; no per-operation OAuth scopes in\n    the spec. App login (not the API) uses OAuth 2.0 / OIDC via Clerk.\nschemes:\n- name: APIKey\n  type: http\n  scheme: bearer\n  description: API key authentication, for service access (Management API)\n  sources:\n  - openapi/bucket-management-openapi-original.json\nkeys:\n  runtime_api:\n  - name: Publishable key\n    usage: client-side (web/mobile/public apps)\n    transport: Authorization Bearer, or ?publishableKey= query parameter\n    scope: environment-specific; safe to expose; limited permissions\n  - name: Secret key\n    usage: server-side only\n    transport: Authorization Bearer only\n    scope:\
  \ environment-specific; grants targeting definitions and secret flags\n  management_api:\n  - name: API key\n    usage: server-side / CI-CD (e.g. Reflag CLI)\n    transport: Authorization Bearer\n    scope: app-scoped, usable across all environments; scoped permissions selected at creation\nidentity_provider:\n  name: Clerk\n  oauth_metadata: https://app.reflag.com/.well-known/oauth-authorization-server\n  oidc_discovery: https://clerk.reflag.com/.well-known/openid-configuration\n  note: OAuth 2.0 / OIDC for dashboard login, not for API access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bucket/refs/heads/main/authentication/bucket-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Feature Flags
- Feature Management
- Feature Flagging
- Developer Tools
- SaaS
- Entitlements
- Experimentation
- MCP
- Agent Ready
---
