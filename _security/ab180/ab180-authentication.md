---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: overview
  format: yaml
  label: Airbridge API
  slug: airbridge-api
  spec_type: Postman
  url: https://www.postman.com/airbridge-engineering/workspace/airbridge-api/overview
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Ab180 Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ab180 secures its APIs with http, apiKey, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ab180
provider_slug: ab180
scheme_count: 3
schemes:
- applies_to: https://api.airbridge.io
  bearer_format: Airbridge API token
  in: header
  issued_at: Airbridge dashboard, [Settings] > [Tokens]
  name: bearerAuth
  parameter: Authorization
  rotation: Regenerating a token in [Settings] > [Tokens] immediately and automatically revokes the existing token; every caller using it starts receiving an unauthorized error.
  scheme: bearer
  source: https://help.airbridge.io/en/references/introduction
  token_types:
  - name: API Token
    scope: All API calls. Broad permission — the docs warn it must not be exposed in publicly accessible areas.
  - name: Tracking Link API Token
    scope: Tracking link generation only. Intended for use from a client or client server.
  type: http
  value_form: 'Authorization: Bearer {AIRBRIDGE-API-TOKEN}'
- applies_to: https://api.airbridge.io/skadnetwork/v1/conversion-value-schema
  in: query
  name: skanApiKey
  note: The SKAdNetwork conversion-value schema endpoint takes its key as a query-string parameter rather than an Authorization header — the one endpoint in the published surface that deviates from bearer auth.
  parameter: api_key
  source: https://help.airbridge.io/en/references/skadnetwork-configuration/response-for-all-versions-of-skan
  type: apiKey
- applies_to: https://mcp.airbridge.io/mcp
  discovery:
  - well-known/ab180-oauth-authorization-server.json
  - well-known/ab180-oauth-protected-resource.json
  - well-known/ab180-openid-configuration.json
  dynamic_client_registration: https://mcp.airbridge.io/register
  flows:
  - authorizationUrl: https://mcp.airbridge.io/oauth/authorize
    flow: authorizationCode
    pkce: S256
    scopes:
      email: Email address claim
      openid: OpenID Connect subject
      profile: Basic profile claims
    tokenUrl: https://mcp.airbridge.io/oauth/token
  id_token_signing_alg:
  - RS256
  method: probed
  name: airbridgeMcpOAuth
  source: https://mcp.airbridge.io/.well-known/oauth-authorization-server
  token_endpoint_auth_methods:
  - none
  type: oauth2
  userinfo_endpoint: https://mcp.airbridge.io/oauth/userinfo
slug: ab180-authentication
source_filename: ab180-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: searched\nsource: openapi/ NONE — derived from provider documentation\ndocs: https://help.airbridge.io/en/references/introduction\nnote: 'Airbridge publishes no OpenAPI, so no securityScheme block could be parsed. This\n  profile is read from the API reference introduction, the per-endpoint reference pages\n  and the live OAuth discovery documents on mcp.airbridge.io.'\nsummary:\n  types:\n  - http\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: Airbridge API token\n  in: header\n  parameter: Authorization\n  applies_to: https://api.airbridge.io\n  value_form: 'Authorization: Bearer {AIRBRIDGE-API-TOKEN}'\n  issued_at: 'Airbridge dashboard, [Settings] > [Tokens]'\n  source: https://help.airbridge.io/en/references/introduction\n  token_types:\n  - name: API Token\n    scope: 'All API calls. Broad permission — the\
  \ docs warn it must not be exposed in\n      publicly accessible areas.'\n  - name: Tracking Link API Token\n    scope: 'Tracking link generation only. Intended for use from a client or client\n      server.'\n  rotation: 'Regenerating a token in [Settings] > [Tokens] immediately and automatically\n    revokes the existing token; every caller using it starts receiving an unauthorized\n    error.'\n- name: skanApiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  applies_to: https://api.airbridge.io/skadnetwork/v1/conversion-value-schema\n  source: https://help.airbridge.io/en/references/skadnetwork-configuration/response-for-all-versions-of-skan\n  note: 'The SKAdNetwork conversion-value schema endpoint takes its key as a query-string\n    parameter rather than an Authorization header — the one endpoint in the published\n    surface that deviates from bearer auth.'\n- name: airbridgeMcpOAuth\n  type: oauth2\n  applies_to: https://mcp.airbridge.io/mcp\n  flows:\n  - flow: authorizationCode\n\
  \    authorizationUrl: https://mcp.airbridge.io/oauth/authorize\n    tokenUrl: https://mcp.airbridge.io/oauth/token\n    pkce: S256\n    scopes:\n      openid: OpenID Connect subject\n      profile: Basic profile claims\n      email: Email address claim\n  dynamic_client_registration: https://mcp.airbridge.io/register\n  token_endpoint_auth_methods:\n  - none\n  userinfo_endpoint: https://mcp.airbridge.io/oauth/userinfo\n  id_token_signing_alg:\n  - RS256\n  discovery:\n  - well-known/ab180-oauth-authorization-server.json\n  - well-known/ab180-oauth-protected-resource.json\n  - well-known/ab180-openid-configuration.json\n  source: https://mcp.airbridge.io/.well-known/oauth-authorization-server\n  method: probed\nsdk_authentication:\n  note: 'Client SDKs authenticate with an app name (unique ID) plus an SDK token, both\n    read from [Settings] > [Tokens] in the dashboard. This is a separate credential from\n    the REST API token.'\n  source: https://help.airbridge.io/en/developers/sdk-quickstart\n\
  transport:\n  https_required: true\n  note: 'All requests must be made over HTTPS; plain HTTP and unauthenticated requests\n    return an error.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ab180/refs/heads/main/authentication/ab180-authentication.yml
summary_line: http/apiKey/oauth2 · 3 schemes
tags:
- Company
- Attribution
- Mobile Measurement
- Marketing
- Analytics
- Advertising
- Deep Linking
- Mobile
- Reporting
- South Korea
---
