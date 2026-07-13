---
api_key_in: []
api_specs:
- filename: auth0-management-api-openapi.yml
  format: yaml
  label: Auth0 Management API
  slug: auth0-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-management-api-openapi.yml
- filename: auth0-authentication-api-openapi.yml
  format: yaml
  label: Auth0 Authentication API
  slug: auth0-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-authentication-api-openapi.yml
- filename: auth0-fga-openapi.yml
  format: yaml
  label: Auth0 FGA (Fine-Grained Authorization)
  slug: auth0-fga
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/openapi/auth0-fga-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Auth0 Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Auth0 secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Auth0
provider_slug: auth0
scheme_count: 2
schemes:
- bearerFormat: jwt
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/auth0-management-api-openapi.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 221
    tokenUrl: /oauth/token/
  name: oAuth2ClientCredentials
  sources:
  - openapi/auth0-management-api-openapi.yml
  type: oauth2
slug: auth0-authentication
source_filename: auth0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/auth0-management-api-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: jwt\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n- name: oAuth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: /oauth/token/\n    scopes: 221\n  sources:\n  - openapi/auth0-management-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/auth0/refs/heads/main/authentication/auth0-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- AI Agents
- Authentication
- Authorization
- FGA
- Identity Management
- MCP
- OAuth
- Okta
- OpenID Connect
- SAML
- Security
- SCIM
---
