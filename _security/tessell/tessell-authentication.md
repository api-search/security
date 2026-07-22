---
api_key_in: []
api_specs:
- filename: tessell-openapi-original.json
  format: json
  label: Tessell API
  slug: tessell-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessell/refs/heads/main/openapi/tessell-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tessell Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tessell secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tessell
provider_slug: tessell
scheme_count: 1
schemes:
- detail: 'Tokens are minted by exchanging tenant credentials for an access token: obtain a Tenant ID and API Key during onboarding, then POST to /iam/authorize with headers tenant-id, content-type: application/json and the API key in the body (operationId authorizeApiKey). The returned token is sent as the Authorization header on every call to https://api.console.tessell.com. API keys themselves are managed via /iam/api-keys (createApiKey, getApiKeys, revokeApiKey). No OAuth 2.0 / OIDC flow is exposed on the public API; console sign-in supports SSO/identity providers separately.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/tessell-openapi-original.json
  type: http
slug: tessell-authentication
source_filename: tessell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/tessell-openapi-original.json\ndocs: https://developer.tessell.com/docs/getting-started\nsummary:\n  types:\n  - http\n  flow: api-key-exchange-to-bearer\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/tessell-openapi-original.json\n  detail: >-\n    Tokens are minted by exchanging tenant credentials for an access token: obtain a Tenant ID and\n    API Key during onboarding, then POST to /iam/authorize with headers tenant-id,\n    content-type: application/json and the API key in the body (operationId authorizeApiKey). The\n    returned token is sent as the Authorization header on every call to\n    https://api.console.tessell.com. API keys themselves are managed via /iam/api-keys\n    (createApiKey, getApiKeys, revokeApiKey). No OAuth 2.0 / OIDC flow is exposed on the public\n    API; console sign-in supports SSO/identity providers separately.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessell/refs/heads/main/authentication/tessell-authentication.yml
summary_line: http · 1 scheme
tags:
- Databases
- DBaaS
- Multi-Cloud
- Oracle
- PostgreSQL
- MySQL
- SQL Server
- Data Infrastructure
---
