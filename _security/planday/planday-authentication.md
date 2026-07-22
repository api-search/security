---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Planday Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Planday secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Planday
provider_slug: planday
scheme_count: 2
schemes:
- description: Access to the Planday API is secured by a standard OAuth2 flow with a bearer token. Apps are registered in the portal (Settings -> API access) with a fixed set of scopes. Access tokens expire after 1 hour; a non-expiring refresh token is used to obtain new access tokens.
  flows:
  - authorizationUrl: https://id.planday.com/connect/authorize
    flow: authorizationCode
    scope_count: 76
    tokenUrl: https://id.planday.com/connect/token
  - flow: clientCredentials
    tokenUrl: https://id.planday.com/connect/token
  - flow: refreshToken
    tokenUrl: https://id.planday.com/connect/token
  name: OAuth2
  scheme: bearer
  source: https://id.planday.com/.well-known/openid-configuration
  type: oauth2
- name: OpenIDConnect
  openIdConnectUrl: https://id.planday.com/.well-known/openid-configuration
  source: https://id.planday.com/.well-known/openid-configuration
  type: openIdConnect
slug: planday-authentication
source_filename: planday-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://id.planday.com/.well-known/openid-configuration\ndocs: https://openapi.planday.com/gettingstarted/authorization-flow/\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  token_endpoint: https://id.planday.com/connect/token\n  authorization_endpoint: https://id.planday.com/connect/authorize\n  access_token_ttl_seconds: 3600\n  refresh_token: non-expiring (until revoked or lost)\n  additional_header: 'X-ClientId: <app id> is required on API calls alongside the bearer token'\nschemes:\n- name: OAuth2\n  type: oauth2\n  scheme: bearer\n  description: 'Access to the Planday API is secured by a standard OAuth2 flow with a\n    bearer token. Apps are registered in the portal (Settings -> API access) with a\n    fixed set of scopes. Access tokens expire after 1 hour; a non-expiring refresh\n    token is used to obtain new access tokens.'\n  source: https://id.planday.com/.well-known/openid-configuration\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://id.planday.com/connect/authorize\n    tokenUrl: https://id.planday.com/connect/token\n    scope_count: 76\n  - flow: clientCredentials\n    tokenUrl: https://id.planday.com/connect/token\n  - flow: refreshToken\n    tokenUrl: https://id.planday.com/connect/token\n- name: OpenIDConnect\n  type: openIdConnect\n  openIdConnectUrl: https://id.planday.com/.well-known/openid-configuration\n  source: https://id.planday.com/.well-known/openid-configuration\ngrant_types_supported:\n- authorization_code\n- client_credentials\n- refresh_token\n- implicit\n- password\n- 'urn:ietf:params:oauth:grant-type:device_code'\n- token_exchange\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/planday/refs/heads/main/authentication/planday-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- SaaS
- Workforce Management
- Scheduling
- Time Tracking
- Payroll
- Human Resources
- Hospitality
- Retail
- REST
- OAuth2
---
