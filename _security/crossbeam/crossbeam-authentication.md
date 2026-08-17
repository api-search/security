---
api_key_in: []
api_specs:
- filename: postman.yaml
  format: yaml
  label: Crossbeam Partner API
  slug: crossbeam-partner-api
  spec_type: Postman
  url: https://developers.crossbeam.com/
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Crossbeam Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Crossbeam secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Crossbeam
provider_slug: crossbeam
scheme_count: 1
schemes:
- access_token_lifetime: 24h
  audience: https://api.getcrossbeam.com
  authorizationUrl: https://auth.crossbeam.com/authorize?audience=https://api.getcrossbeam.com
  flow: authorizationCode
  name: OAuth2
  refresh: Request the offline_access scope to receive a refresh token; exchange it at the token URL with grant_type=refresh_token for long-running integrations.
  sources:
  - docs
  tokenUrl: https://auth.crossbeam.com/oauth/token
  type: oauth2
slug: crossbeam-authentication
source_filename: crossbeam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://developers.crossbeam.com/\ndocs:\n  - https://developers.crossbeam.com/\n  - https://help.crossbeam.com/en/articles/4677142-rest-api\n  - https://gitlab.com/crossbeam-public/crossbeam-simple-oauth2\ndiscovery:\n  openid_configuration: https://auth.crossbeam.com/.well-known/openid-configuration\n  oauth_authorization_server: https://auth.crossbeam.com/.well-known/oauth-authorization-server\n  jwks_uri: https://auth.crossbeam.com/.well-known/jwks.json\n  probed: '2026-08-14'\n  http_status: 200\n  artifact: well-known/crossbeam-openid-configuration.json\n  note: >-\n    Verified live. The authorization server is an Auth0 custom domain. Discovery advertises\n    PKCE (S256), a device-authorization endpoint, dynamic client registration, revocation, and\n    grant types authorization_code / refresh_token / client_credentials / device_code /\n    implicit / password. token_endpoint_auth_methods_supported includes private_key_jwt.\n\
  summary:\n  types: [oauth2]\n  oauth2_flows: [authorizationCode]\n  api_key_in: []\n  note: >-\n    Public Crossbeam Partner API uses standard OAuth 2.0 (three-legged, authorization-code).\n    Credentials are created as a Custom Integration app in the Crossbeam UI\n    (https://app.crossbeam.com/integrations), which issues a Client ID and Client Secret.\n    Positioned for Enterprise customers.\nschemes:\n  - name: OAuth2\n    type: oauth2\n    flow: authorizationCode\n    authorizationUrl: https://auth.crossbeam.com/authorize?audience=https://api.getcrossbeam.com\n    tokenUrl: https://auth.crossbeam.com/oauth/token\n    audience: https://api.getcrossbeam.com\n    access_token_lifetime: 24h\n    refresh: >-\n      Request the offline_access scope to receive a refresh token; exchange it at the token\n      URL with grant_type=refresh_token for long-running integrations.\n    sources: [docs]\nrequired_headers:\n  - name: Authorization\n    value: 'Bearer <access_token>'\n    required:\
  \ true\n  - name: Xbeam-Organization\n    value: '<organization-uuid>'\n    required: true\n    note: >-\n      Selects which organization's data to return (a user may belong to multiple orgs).\n      Obtain the uuid from GET /v1/users/me (Crossbeam's prose still says /v0.1/users/me, but\n      the runnable request in its own collection is /v1). Omitting this header is the most\n      common cause of 4xx errors.\nmcp_authentication:\n  endpoint: https://mcp.crossbeam.com/mcp\n  type: oauth2\n  discovery:\n    protected_resource: https://mcp.crossbeam.com/.well-known/oauth-protected-resource\n    authorization_server: https://mcp.crossbeam.com/.well-known/oauth-authorization-server\n  probed: '2026-08-14'\n  note: >-\n    The remote MCP server runs its OWN authorization server (authorize / oauth/token / register\n    on mcp.crossbeam.com) with dynamic client registration and PKCE, while validating against\n    the same JWKS as the REST API (auth.crossbeam.com/.well-known/jwks.json). Its\
  \ scope set\n    (openid, profile, email, offline_access) is the OIDC baseline — the read:partnerships /\n    read:reports / read:populations scopes that gate the REST API are not exposed at the MCP\n    authorization layer.\n  artifacts:\n    - well-known/crossbeam-mcp-oauth-protected-resource.json\n    - well-known/crossbeam-mcp-oauth-authorization-server.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossbeam/refs/heads/main/authentication/crossbeam-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Ecosystem-Led Growth
- Partnerships
- Account Mapping
- Co-Selling
- Data Collaboration
- Sales Intelligence
- CRM
- Webhooks
- MCP
---
