---
api_key_in: []
api_specs:
- filename: showpad-v3-openapi-original.yml
  format: yaml
  label: Showpad Content API
  slug: showpad-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/openapi/showpad-v3-openapi-original.yml
- filename: showpad-v4-openapi-original.yml
  format: yaml
  label: Showpad API v4
  slug: showpad-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/openapi/showpad-v4-openapi-original.yml
- filename: showpad-v3-openapi-original.yml
  format: yaml
  label: Showpad User Management API
  slug: showpad-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/openapi/showpad-v3-openapi-original.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Showpad Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- password
- refresh_token
overview: Showpad secures its APIs with http and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, password, and refresh_token flow(s).
provider_name: Showpad
provider_slug: showpad
scheme_count: 3
schemes:
- description: Bearer token identifying the requesting user. Accepts either an OAuth 2.0 access token or a personal API token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/showpad-v3-openapi-original.yml
  - openapi/showpad-v4-openapi-original.yml
  type: http
- docs: https://developer.showpad.com/docs/apis/concepts/authentication
  flows:
  - authorizationUrl: https://{subdomain}.showpad.biz/api/v3/oauth2/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://{subdomain}.showpad.biz/api/v3/oauth2/token
  - flow: password
    scopes: 7
    tokenUrl: https://{subdomain}.showpad.biz/api/v3/oauth2/token
  name: oAuth
  sources:
  - openapi/showpad-v3-openapi-original.yml
  type: oauth2
- flows:
  - authorizationUrl: https://mcp.showpad.com/oauth/v1/auth
    code_challenge_methods:
    - S256
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://mcp.showpad.com/oauth/v1/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://mcp.showpad.com
  name: Showpad MCP OAuth
  sources:
  - well-known/showpad-oauth-authorization-server.json
  - well-known/showpad-oauth-protected-resource.json
  surface: mcp
  token_endpoint_auth_methods:
  - none
  - client_secret_post
  type: oauth2
slug: showpad-authentication
source_filename: showpad-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: openapi/showpad-v3-openapi-original.yml, openapi/showpad-v4-openapi-original.yml\ndocs: https://developer.showpad.com/docs/apis/concepts/authentication\nsummary:\n  types: [http, oauth2]\n  http_schemes: [bearer]\n  oauth2_flows: [authorizationCode, password, refresh_token]\n  api_key_in: []\n  header: 'Authorization: Bearer <token>'\n  tenant_scoped: true\n  tenant_note: >-\n    Every authentication endpoint is tenant-scoped to the customer's Showpad subdomain; there\n    is no shared authorization host for the REST API.\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      Bearer token identifying the requesting user. Accepts either an OAuth 2.0 access token\n      or a personal API token.\n    sources:\n      - openapi/showpad-v3-openapi-original.yml\n      - openapi/showpad-v4-openapi-original.yml\n  - name: oAuth\n    type: oauth2\n    flows:\n      - flow: authorizationCode\n\
  \        authorizationUrl: https://{subdomain}.showpad.biz/api/v3/oauth2/authorize\n        tokenUrl: https://{subdomain}.showpad.biz/api/v3/oauth2/token\n        scopes: 6\n      - flow: password\n        tokenUrl: https://{subdomain}.showpad.biz/api/v3/oauth2/token\n        scopes: 7\n    sources:\n      - openapi/showpad-v3-openapi-original.yml\n    docs: https://developer.showpad.com/docs/apis/concepts/authentication\n  - name: Showpad MCP OAuth\n    type: oauth2\n    surface: mcp\n    issuer: https://mcp.showpad.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://mcp.showpad.com/oauth/v1/auth\n        tokenUrl: https://mcp.showpad.com/oauth/v1/token\n        code_challenge_methods: [S256]\n        scopes: 7\n    token_endpoint_auth_methods: [none, client_secret_post]\n    grant_types: [authorization_code, refresh_token]\n    sources:\n      - well-known/showpad-oauth-authorization-server.json\n      - well-known/showpad-oauth-protected-resource.json\n\
  methods:\n  - name: OAuth 2.0 Authorization Code\n    use: Server-side apps where users log in with their Showpad credentials.\n  - name: OAuth 2.0 Refresh Token\n    use: Obtaining new access tokens when the current one expires.\n  - name: OAuth 2.0 User Credentials (password grant)\n    use: Backend services that control both the application and the user credentials.\n  - name: Personal API Token\n    use: >-\n      Direct API access without an OAuth flow. Generated in Admin App -> Settings -> API\n      Tokens with a descriptive name and an optional expiry date. Displayed once only.\ntoken_lifetimes:\n  access_token: 1 hour\n  refresh_token: 14 days\n  refresh_token_configurable: true\n  refresh_token_configurable_note: Set per OAuth client at registration.\n  personal_api_token: optional expiry set at creation\nclient_registration:\n  location: Admin App -> Settings -> Manage OAuth Clients\n  fields:\n    - client name\n    - redirect URL\n    - description\n    - website\n    - scope\
  \ selections\n    - refresh token lifetime\n  issued:\n    - Client ID\n    - Client Secret\n  self_serve: false\n  self_serve_note: >-\n    OAuth client registration requires administrator access to a provisioned Showpad\n    organization. There is no public developer signup.\nenterprise_identity:\n  sso: SAML 2.0\n  provisioning: SCIM 2.0\n  scim_base: https://{subdomain}.showpad.biz/api/Users/scim/v2\n  scim_docs: https://developer.showpad.com/docs/apis/users/SCIM\n  idps_documented: [Okta, Azure AD, OneLogin, Ping Identity, Salesforce, Microsoft AD FS]\nscopes: scopes/showpad-scopes.yml\nerror_handling:\n  '401': Missing or invalid authentication token.\n  '403': Valid token but insufficient permissions.\n  see: errors/showpad-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/showpad/refs/heads/main/authentication/showpad-authentication.yml
summary_line: http/oauth2 · 3 schemes
tags:
- Sales Enablement
- Sales Coaching
- Content Management
- Buyer Engagement
- Sales Analytics
- Training
- CRM Integration
- Digital Sales Rooms
- Model Context Protocol
- SCIM
---
