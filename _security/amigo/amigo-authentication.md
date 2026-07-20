---
api_key_in:
- header
api_specs:
- filename: amigo-classic-openapi-original.json
  format: json
  label: Amigo Classic API
  slug: amigo-classic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amigo/refs/heads/main/openapi/amigo-classic-openapi-original.json
- filename: amigo-platform-openapi-original.json
  format: json
  label: Amigo Platform API
  slug: amigo-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amigo/refs/heads/main/openapi/amigo-platform-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Amigo Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Amigo secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Amigo
provider_slug: amigo
scheme_count: 3
schemes:
- bearerFormat: JWT
  description: Amigo issued JWT token that identifies an user. It's issued either after logging in through the frontend, or manually through the [`SignInWithAPIKey`](sign-in-with-api-key) endpoint.
  name: Bearer-Authorization
  scheme: bearer
  sources:
  - openapi/amigo-classic-openapi-original.json
  - openapi/amigo-platform-openapi-original.json
  type: http
- description: An optional organization identifier that indicates from which organization the token is issued. This is used in rare cases where the user to authenticate is making a request for resources in another organization.
  in: header
  name: Bearer-Authorization-Organization
  parameter: X-ORG-ID
  sources:
  - openapi/amigo-classic-openapi-original.json
  type: apiKey
- description: The username should be set to {org_id}_{user_id}, and the password should be the Amigo issued JWT token that identifies the user.
  name: Basic
  scheme: basic
  sources:
  - openapi/amigo-classic-openapi-original.json
  type: http
slug: amigo-authentication
source_filename: amigo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: openapi/amigo-classic-openapi-original.json, openapi/amigo-platform-openapi-original.json\ndocs:\n  - https://docs.amigo.ai/developer-guide/getting-started/authentication.md\n  - https://docs.amigo.ai/developer-guide/platform-api/platform-api/oauth2.md\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Classic API uses organization-scoped JWT bearer (obtained via sign-in-with-api-key /\n    sign-in-with-email) plus an optional X-ORG-ID header and a Basic variant. Platform API\n    uses a workspace-scoped API key as a Bearer token OR OAuth2 client_credentials (M2M) at\n    https://identity.platform.amigo.ai/token (3600s access tokens, 53 scopes — see\n    scopes/amigo-scopes.yml). The published OpenAPI declares http bearer schemes only; the\n    OAuth2 flow is documented in the auth docs and OIDC discovery, not the spec.\nschemes:\n- name:\
  \ Bearer-Authorization\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Amigo issued JWT token that identifies an user. It's issued either after logging\n    in through the frontend, or manually through the [`SignInWithAPIKey`](sign-in-with-api-key)\n    endpoint.\n  sources:\n  - openapi/amigo-classic-openapi-original.json\n  - openapi/amigo-platform-openapi-original.json\n- name: Bearer-Authorization-Organization\n  type: apiKey\n  in: header\n  parameter: X-ORG-ID\n  description: An optional organization identifier that indicates from which organization the\n    token is issued. This is used in rare cases where the user to authenticate is making a request\n    for resources in another organization.\n  sources:\n  - openapi/amigo-classic-openapi-original.json\n- name: Basic\n  type: http\n  scheme: basic\n  description: The username should be set to {org_id}_{user_id}, and the password should be\n    the Amigo issued JWT token that identifies the user.\n  sources:\n\
  \  - openapi/amigo-classic-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amigo/refs/heads/main/authentication/amigo-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Ai
- Healthcare
- AI Agents
- Voice
- Clinical
- Conversational AI
- FHIR
- EHR
- HIPAA
---
