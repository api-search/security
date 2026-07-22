---
api_key_in:
- header
api_specs:
- filename: pendoio-engage-openapi.yml
  format: yaml
  label: Pendo Engage API
  slug: pendo-engage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/openapi/pendoio-engage-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pendoio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Pendo.io secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Pendo.io
provider_slug: pendoio
scheme_count: 2
schemes:
- description: Primary Engage API authentication. A per-subscription integration key created at https://app.pendo.io/admin/integrationkeys, sent in the x-pendo-integration-key request header. Verify a key with GET /api/v1/token/verify.
  in: header
  name: IntegrationKey
  parameter: x-pendo-integration-key
  sources:
  - openapi/pendoio-engage-openapi.yml
  type: apiKey
- code_challenge_methods_supported:
  - S256
  description: Pendo publishes RFC 8414 OAuth 2.0 Authorization Server metadata at https://app.pendo.io/.well-known/oauth-authorization-server. Supports the authorization_code (with PKCE S256), refresh_token, and client_credentials grants, plus RFC 7591 Dynamic Client Registration.
  flows:
  - authorizationUrl: https://app.pendo.io/oauth/authorize
    flow: authorizationCode
    tokenUrl: https://app.pendo.io/oauth/v1/token
  - flow: clientCredentials
    tokenUrl: https://app.pendo.io/oauth/v1/token
  name: OAuth2
  registration_endpoint: https://app.pendo.io/oauth/v1/register
  sources:
  - well-known/pendoio-oauth-authorization-server.json
  type: oauth2
  userinfo_endpoint: https://app.pendo.io/oauth/v1/userinfo
slug: pendoio-authentication
source_filename: pendoio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/pendoio-engage-openapi.yml\ndocs: https://app.pendo.io/admin/integrationkeys\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: IntegrationKey\n  type: apiKey\n  in: header\n  parameter: x-pendo-integration-key\n  description: >-\n    Primary Engage API authentication. A per-subscription integration key created at\n    https://app.pendo.io/admin/integrationkeys, sent in the x-pendo-integration-key\n    request header. Verify a key with GET /api/v1/token/verify.\n  sources:\n  - openapi/pendoio-engage-openapi.yml\n- name: OAuth2\n  type: oauth2\n  description: >-\n    Pendo publishes RFC 8414 OAuth 2.0 Authorization Server metadata at\n    https://app.pendo.io/.well-known/oauth-authorization-server. Supports the\n    authorization_code (with PKCE S256), refresh_token, and client_credentials\n    grants, plus RFC 7591\
  \ Dynamic Client Registration.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.pendo.io/oauth/authorize\n    tokenUrl: https://app.pendo.io/oauth/v1/token\n  - flow: clientCredentials\n    tokenUrl: https://app.pendo.io/oauth/v1/token\n  registration_endpoint: https://app.pendo.io/oauth/v1/register\n  userinfo_endpoint: https://app.pendo.io/oauth/v1/userinfo\n  code_challenge_methods_supported:\n  - S256\n  sources:\n  - well-known/pendoio-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pendoio/refs/heads/main/authentication/pendoio-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Product Analytics
- Product Experience
- Digital Adoption
- User Analytics
- In-App Guidance
- Customer Feedback
- SaaS
---
