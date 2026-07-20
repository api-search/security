---
api_key_in:
- header
api_specs:
- filename: dash0-openapi.json
  format: json
  label: Dash0 API
  slug: dash0-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dash0/refs/heads/main/openapi/dash0-openapi.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Dash0 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: Dash0 secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: Dash0
provider_slug: dash0
scheme_count: 2
schemes:
- description: Primary API authentication. A Dash0 auth token (created in the org settings) is sent as a bearer token in the Authorization header. Edge collectors and the CLI use the same token model; the token scopes requests to the owning organization.
  location: 'Authorization: Bearer <DASH0_AUTH_TOKEN>'
  name: BearerAuth
  scheme: bearer
  type: http
- description: OAuth 2.0 (RFC 6749) with PKCE and dynamic client registration (RFC 7591), used by the CLI browser login and by MCP clients. Token endpoint auth method is `none` (public clients + PKCE). Refresh tokens are supported.
  flows:
  - authorizationUrl: https://api.<region>.aws.dash0.com/oauth/authorize
    dynamic_client_registration: true
    flow: authorizationCode
    pkce: S256
    registrationUrl: https://api.<region>.aws.dash0.com/oauth/register
    revocationUrl: https://api.<region>.aws.dash0.com/oauth/revoke
    scopes:
      '*': Full-access wildcard scope (the only scope Dash0 advertises today).
    tokenUrl: https://api.<region>.aws.dash0.com/oauth/token
    userinfoUrl: https://api.<region>.aws.dash0.com/oauth/userinfo
  name: OAuth2
  type: oauth2
slug: dash0-authentication
source_filename: dash0-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api-docs.dash0.com/ + live /.well-known/oauth-authorization-server\ndocs: https://www.dash0.com/docs/dash0\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode, refreshToken]\n  api_key_in: [header]\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  location: 'Authorization: Bearer <DASH0_AUTH_TOKEN>'\n  description: >-\n    Primary API authentication. A Dash0 auth token (created in the org settings)\n    is sent as a bearer token in the Authorization header. Edge collectors and\n    the CLI use the same token model; the token scopes requests to the owning\n    organization.\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.<region>.aws.dash0.com/oauth/authorize\n    tokenUrl: https://api.<region>.aws.dash0.com/oauth/token\n    revocationUrl: https://api.<region>.aws.dash0.com/oauth/revoke\n    registrationUrl:\
  \ https://api.<region>.aws.dash0.com/oauth/register\n    userinfoUrl: https://api.<region>.aws.dash0.com/oauth/userinfo\n    pkce: S256\n    dynamic_client_registration: true\n    scopes:\n      '*': Full-access wildcard scope (the only scope Dash0 advertises today).\n  description: >-\n    OAuth 2.0 (RFC 6749) with PKCE and dynamic client registration (RFC 7591),\n    used by the CLI browser login and by MCP clients. Token endpoint auth method\n    is `none` (public clients + PKCE). Refresh tokens are supported.\nnotes: >-\n  The published OpenAPI does not declare securitySchemes at the document level;\n  auth is documented in the API docs and discoverable via the OAuth\n  Authorization Server / Protected Resource metadata endpoints. Regional hosts:\n  eu-west-1 / eu-central-1 / us-west-2 (AWS), europe-west4 (GCP).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dash0/refs/heads/main/authentication/dash0-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Observability
- OpenTelemetry
- Monitoring
- Logs
- Metrics
- Tracing
- APM
- Prometheus
- DevOps
- Company
- Apis
---
