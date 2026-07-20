---
api_key_in: []
api_specs:
- filename: coactive-ai-openapi-original.json
  format: json
  label: Coactive AI API
  slug: coactive-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coactive-ai/refs/heads/main/openapi/coactive-ai-openapi-original.json
auth_types:
- http
description: 'Coactive uses HTTP Bearer access tokens. A short-lived (3600s) access token is obtained from POST /api/v0/login by exchanging either a personal token (grant_type refresh_token, presented as a Bearer) or system credentials (grant_type client_credentials, CLIENT_ID:CLIENT_SECRET via HTTP Basic). The resulting access_token is sent as `Authorization: Bearer <token>` on every request. Access is governed by RBAC roles; SSO/SAML is available for login.'
kind: authentication
layout: security
method: searched
name: Coactive Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coactive AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Coactive AI
provider_slug: coactive-ai
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/coactive-ai-openapi-original.json
  type: http
slug: coactive-ai-authentication
source_filename: coactive-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.coactive.ai/api-reference/authentication/api-authentication\ndocs: https://docs.coactive.ai/api-reference/authentication/api-authentication\ndescription: >-\n  Coactive uses HTTP Bearer access tokens. A short-lived (3600s) access token is\n  obtained from POST /api/v0/login by exchanging either a personal token\n  (grant_type refresh_token, presented as a Bearer) or system credentials\n  (grant_type client_credentials, CLIENT_ID:CLIENT_SECRET via HTTP Basic).\n  The resulting access_token is sent as `Authorization: Bearer <token>` on every\n  request. Access is governed by RBAC roles; SSO/SAML is available for login.\nsummary:\n  types:\n  - http\n  token_endpoint: /api/v0/login\n  grant_types:\n  - client_credentials\n  - refresh_token\n  access_token_ttl_seconds: 3600\n  credential_types:\n  - personal_token\n  - system_credentials\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  -\
  \ openapi/coactive-ai-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coactive-ai/refs/heads/main/authentication/coactive-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Multimodal AI
- Computer Vision
- Video Understanding
- Image Search
- Contextual Advertising
- Media
- Content Moderation
- Metadata
---
