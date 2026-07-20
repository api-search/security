---
api_key_in:
- header
api_specs:
- filename: fortify-software-fod-openapi.json
  format: json
  label: Fortify on Demand REST API (v3)
  slug: fortify-on-demand-rest-api-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortify-software/refs/heads/main/openapi/fortify-software-fod-openapi.json
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Fortify Software Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Fortify Software secures its APIs with oauth2 and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Fortify Software
provider_slug: fortify-software
scheme_count: 4
schemes:
- description: OAuth 2.0 client-credentials grant. Exchange an API key (client_id) and secret (client_secret), or a Personal Access Token, at the token endpoint for a bearer access token. Scope requested via the `scope` parameter gates which operations the token may call.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  scopes_ref: scopes/fortify-software-scopes.yml
  sources:
  - docs
  - openapi/fortify-software-fod-openapi.json
  tokenUrl: https://api.ams.fortify.com/oauth/token
  type: oauth2
- bearerFormat: JWT
  description: 'Access token returned by the token endpoint is presented as `Authorization: Bearer <access_token>` on every API call.'
  name: BearerToken
  scheme: bearer
  sources:
  - docs
  type: http
- description: Personal Access Tokens (PATs) are created per user with a scope set and can be exchanged for a bearer token via the client-credentials grant (grant_type password / scope). Managed via the PersonalAccessTokens API resource.
  in: header
  name: PersonalAccessToken
  parameter: Authorization
  sources:
  - docs
  - openapi/fortify-software-fod-openapi.json
  type: apiKey
- description: Tenant-level API keys (client credentials) managed through the ApiKeyManagement resource; used as client_id/client_secret for the client-credentials grant.
  in: header
  name: TenantApiKey
  parameter: Authorization
  sources:
  - docs
  - openapi/fortify-software-fod-openapi.json
  type: apiKey
slug: fortify-software-authentication
source_filename: fortify-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://api.ams.fortify.com/swagger/ui/index\ndocs: https://www.microfocus.com/documentation/fortify-on-demand/\nnotes: >-\n  The Fortify on Demand v3 Swagger document does not declare securityDefinitions,\n  but the published API documentation and every operation description (\"Allowed\n  Scopes: ...\") document the real authentication model. FoD supports OAuth 2.0\n  client-credentials grant against a token endpoint, plus Personal Access Tokens\n  (managed via the PersonalAccessTokens resource) and tenant API keys (managed via\n  the ApiKeyManagement resource). Scopes gate each operation; see\n  scopes/fortify-software-scopes.yml.\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://api.ams.fortify.com/oauth/token\n  description: >-\n    OAuth 2.0 client-credentials grant.\
  \ Exchange an API key (client_id) and secret\n    (client_secret), or a Personal Access Token, at the token endpoint for a bearer\n    access token. Scope requested via the `scope` parameter gates which operations\n    the token may call.\n  scopes_ref: scopes/fortify-software-scopes.yml\n  sources: [docs, openapi/fortify-software-fod-openapi.json]\n- name: BearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    Access token returned by the token endpoint is presented as\n    `Authorization: Bearer <access_token>` on every API call.\n  sources: [docs]\n- name: PersonalAccessToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Personal Access Tokens (PATs) are created per user with a scope set and can be\n    exchanged for a bearer token via the client-credentials grant (grant_type\n    password / scope). Managed via the PersonalAccessTokens API resource.\n  sources: [docs, openapi/fortify-software-fod-openapi.json]\n-\
  \ name: TenantApiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Tenant-level API keys (client credentials) managed through the ApiKeyManagement\n    resource; used as client_id/client_secret for the client-credentials grant.\n  sources: [docs, openapi/fortify-software-fod-openapi.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortify-software/refs/heads/main/authentication/fortify-software-authentication.yml
summary_line: oauth2/apiKey · 4 schemes
tags:
- Company
- Security
- Application Security
- AppSec
- SAST
- DAST
- Vulnerability Management
- DevSecOps
- Software Composition Analysis
- API Security
---
