---
anonymous_access: false
api_key_in: []
auth_types: []
description: Apollo Global Management's only discoverable authentication surface is the OAuth 2.0 / OpenID Connect authorization server on api.apollo.com that fronts its MCP endpoint. It is an authorization-code + PKCE public-client flow with open dynamic client registration. There is no API-key surface, no mutual-TLS surface, and no published developer authentication guide.
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: Apollo Global Management Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apollo Global Management declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Apollo Global Management
provider_slug: apollo-global-management
scheme_count: 1
schemes:
- authorization_url: https://api.apollo.com/mcp/authorize
  bearer_methods:
  - header
  client_authentication:
  - none
  client_type: public
  dynamic_client_registration: true
  dynamic_client_registration_spec: RFC 7591
  evidence: https://api.apollo.com/.well-known/oauth-authorization-server
  flow: authorizationCode
  id: apollo_mcp_oauth2
  issuer: https://api.apollo.com
  pkce: required
  pkce_methods:
  - S256
  protected_resources:
  - metadata: https://api.apollo.com/.well-known/oauth-protected-resource/mcp
    resource: https://api.apollo.com/mcp
    scopes:
    - openid
    - profile
    - email
  refresh_tokens: true
  registration_url: https://api.apollo.com/mcp/register
  scopes:
  - openid
  - profile
  - email
  - offline_access
  token_url: https://api.apollo.com/mcp/token
  type: oauth2
slug: apollo-global-management-authentication
source_filename: apollo-global-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: >-\n  https://api.apollo.com/.well-known/oauth-authorization-server and\n  https://api.apollo.com/.well-known/oauth-protected-resource/mcp, both HTTP 200\n  application/json, fetched 2026-09-04. Apollo publishes no authentication documentation\n  page; this profile is read entirely from the machine-readable discovery documents.\ndescription: >-\n  Apollo Global Management's only discoverable authentication surface is the OAuth 2.0 /\n  OpenID Connect authorization server on api.apollo.com that fronts its MCP endpoint. It\n  is an authorization-code + PKCE public-client flow with open dynamic client\n  registration. There is no API-key surface, no mutual-TLS surface, and no published\n  developer authentication guide.\nschemes:\n  - id: apollo_mcp_oauth2\n    type: oauth2\n    flow: authorizationCode\n    issuer: https://api.apollo.com\n    authorization_url: https://api.apollo.com/mcp/authorize\n    token_url: https://api.apollo.com/mcp/token\n\
  \    registration_url: https://api.apollo.com/mcp/register\n    pkce: required\n    pkce_methods:\n      - S256\n    client_authentication:\n      - none\n    client_type: public\n    dynamic_client_registration: true\n    dynamic_client_registration_spec: RFC 7591\n    refresh_tokens: true\n    scopes:\n      - openid\n      - profile\n      - email\n      - offline_access\n    bearer_methods:\n      - header\n    protected_resources:\n      - resource: https://api.apollo.com/mcp\n        scopes:\n          - openid\n          - profile\n          - email\n        metadata: https://api.apollo.com/.well-known/oauth-protected-resource/mcp\n    evidence: https://api.apollo.com/.well-known/oauth-authorization-server\nidentity_providers:\n  - name: Okta\n    host: api.apollo.com\n    evidence: >-\n      GET https://api.apollo.com/.well-known/oauth-protected-resource returns 302 to\n      /login/okta?next=... — the interactive login behind this authorization server is\n      Okta-backed.\n\
  \  - name: Okta (apolloid.okta.com)\n    host: client.apollo.com\n    org: https://apolloid.okta.com/oauth2/ausyhvwbuxKgY0uyZ4x7\n    evidence: https://client.apollo.com/.well-known/oauth-protected-resource\n    note: >-\n      Apollo's client/investor portal identity. The resource it protects (`api://vega-mcp`)\n      belongs to the third-party Vega AltOS platform, not to Apollo — recorded for\n      completeness, not claimed as an Apollo contract.\ngaps:\n  - No published authentication documentation page for any Apollo API.\n  - No API-key or personal-access-token surface found.\n  - >-\n    Scope semantics beyond the four standard OIDC/offline_access values are not published;\n    what an Apollo access token actually authorizes cannot be determined from public\n    documents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apollo-global-management/refs/heads/main/authentication/apollo-global-management-authentication.yml
summary_line: 1 scheme
tags:
- Alternative Investments
- Asset Management
- Credit
- Finance
- Investment Management
- Private Equity
- Real Assets
---
