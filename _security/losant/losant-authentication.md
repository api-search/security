---
api_key_in: []
api_specs:
- filename: losant-application-api-openapi.yml
  format: yaml
  label: Losant Application API
  slug: losant-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-application-api-openapi.yml
- filename: losant-device-api-openapi.yml
  format: yaml
  label: Losant Device API
  slug: losant-device-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-device-api-openapi.yml
- filename: losant-experience-api-openapi.yml
  format: yaml
  label: Losant Experience API
  slug: losant-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-experience-api-openapi.yml
- filename: losant-authentication-and-account-api-openapi.yml
  format: yaml
  label: Losant Authentication and Account API
  slug: losant-authentication-and-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-authentication-and-account-api-openapi.yml
- filename: losant-data-and-data-tables-api-openapi.yml
  format: yaml
  label: Losant Data and Data Tables API
  slug: losant-data-and-data-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-data-and-data-tables-api-openapi.yml
- filename: losant-edge-and-embedded-compute-api-openapi.yml
  format: yaml
  label: Losant Edge and Embedded Compute API
  slug: losant-edge-and-embedded-compute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-edge-and-embedded-compute-api-openapi.yml
- filename: losant-enterprise-instance-api-openapi.yml
  format: yaml
  label: Losant Enterprise Instance API
  slug: losant-enterprise-instance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-enterprise-instance-api-openapi.yml
- filename: losant-notebooks-api-openapi.yml
  format: yaml
  label: Losant Notebooks API
  slug: losant-notebooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-notebooks-api-openapi.yml
- filename: losant-workflow-engine-api-openapi.yml
  format: yaml
  label: Losant Workflow Engine API
  slug: losant-workflow-engine-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/openapi/losant-workflow-engine-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Losant Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Losant secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Losant
provider_slug: losant
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: Losant uses JSON Web Tokens (JWTs) for authentication. Obtain a token via POST /auth/user, POST /auth/device, POST /applications/{applicationId}/tokens, or POST /me/tokens and pass it in the Authorization header as `Bearer <token>`.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/losant-application-api-openapi.yml
  - openapi/losant-authentication-and-account-api-openapi.yml
  - openapi/losant-data-and-data-tables-api-openapi.yml
  - openapi/losant-device-api-openapi.yml
  - openapi/losant-edge-and-embedded-compute-api-openapi.yml
  - openapi/losant-enterprise-instance-api-openapi.yml
  - openapi/losant-experience-api-openapi.yml
  - openapi/losant-notebooks-api-openapi.yml
  - openapi/losant-workflow-engine-api-openapi.yml
  type: http
- description: OAuth 2.0 authorization code with PKCE (S256) for third-party applications acting on a user's behalf; the flow behind the hosted MCP server at https://mcp.losant.com/mcp. Dynamic client registration is supported at https://api.losant.com/oauth/clients.
  flows:
  - authorizationUrl: https://accounts.losant.com/oauth
    flow: authorizationCode
    pkce: S256
    revocationUrl: https://api.losant.com/oauth/revoke
    scopes_count: 7
    tokenUrl: https://api.losant.com/oauth/token
  name: OAuth2
  sources:
  - https://api.losant.com/.well-known/oauth-authorization-server
  - https://docs.losant.com/user-accounts/oauth-tokens/
  type: oauth2
slug: losant-authentication
source_filename: losant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: 'https://docs.losant.com/rest-api/overview/ + https://docs.losant.com/user-accounts/oauth-tokens/ + https://api.losant.com/.well-known/oauth-authorization-server\n  (derived baseline: openapi/*.yml)'\nsummary:\n  types:\n  - http\n  - oauth2\n  http_schemes:\n  - bearer\n  oauth2_flows:\n  - authorizationCode\n  note: The OpenAPI files declare only the http bearer scheme. OAuth 2.0 is real but lives outside the specs - it\n    is published in the RFC 8414 authorization-server metadata and used by the hosted MCP server.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Losant uses JSON Web Tokens (JWTs) for authentication. Obtain a token via POST /auth/user, POST /auth/device,\n    POST /applications/{applicationId}/tokens, or POST /me/tokens and pass it in the Authorization header as `Bearer\n    <token>`.\n  sources:\n  - openapi/losant-application-api-openapi.yml\n  - openapi/losant-authentication-and-account-api-openapi.yml\n\
  \  - openapi/losant-data-and-data-tables-api-openapi.yml\n  - openapi/losant-device-api-openapi.yml\n  - openapi/losant-edge-and-embedded-compute-api-openapi.yml\n  - openapi/losant-enterprise-instance-api-openapi.yml\n  - openapi/losant-experience-api-openapi.yml\n  - openapi/losant-notebooks-api-openapi.yml\n  - openapi/losant-workflow-engine-api-openapi.yml\n- name: OAuth2\n  type: oauth2\n  description: OAuth 2.0 authorization code with PKCE (S256) for third-party applications acting on a user's behalf;\n    the flow behind the hosted MCP server at https://mcp.losant.com/mcp. Dynamic client registration is supported\n    at https://api.losant.com/oauth/clients.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.losant.com/oauth\n    tokenUrl: https://api.losant.com/oauth/token\n    revocationUrl: https://api.losant.com/oauth/revoke\n    scopes_count: 7\n    pkce: S256\n  sources:\n  - https://api.losant.com/.well-known/oauth-authorization-server\n  - https://docs.losant.com/user-accounts/oauth-tokens/\n\
  docs: https://docs.losant.com/rest-api/overview/\ntoken_types:\n- name: User API Token\n  obtained_via: POST /auth/user or userApiTokens.post (POST /me/tokens)\n  scope: all.User by default; narrowable per-operation\n  docs: https://docs.losant.com/user-accounts/user-tokens/\n- name: Application API Token\n  obtained_via: applicationApiTokens.post (POST /applications/{applicationId}/tokens)\n  scope: all.Application by default; cannot leave the application\n  docs: https://docs.losant.com/applications/application-tokens/\n- name: Device Token\n  obtained_via: POST /auth/device with deviceId + application key/secret\n  scope: all.Device\n  docs: https://docs.losant.com/rest-api/auth/\n- name: Instance API Token\n  obtained_via: instanceApiTokens.post (POST /instances/{instanceId}/tokens)\n  scope: instance administration\n  docs: https://docs.losant.com/instance-manager/instance-tokens/\n- name: User OAuth Token\n  obtained_via: OAuth 2.0 authorization code flow with user consent\n  scope:\
  \ one or more of the seven OAuth scopes\n  docs: https://docs.losant.com/user-accounts/oauth-tokens/\ntransport:\n  header: 'Authorization: Bearer <token>'\n  mqtt: Devices authenticate to broker.losant.com with an application key as MQTT username and the secret as password,\n    or with an X.509 client certificate.\nmfa:\n  supported: true\n  standard: RFC 6238 TOTP\n  source: https://docs.losant.com/references/security/\ntoken_storage: Losant does not store issued API tokens; scope is encrypted into the token itself and verified server-side,\n  so a lost token cannot be recovered - only revoked.\nscopes_artifact: scopes/losant-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/losant/refs/heads/main/authentication/losant-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- IoT
- Internet of Things
- Devices
- Edge Compute
- Embedded
- MQTT
- Industrial IoT
- Telemetry
- Workflow-Automation
- Visual Workflow Engine
- Dashboards
- Time Series
- Connected Products
- Enterprise
---
