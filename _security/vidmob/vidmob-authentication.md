---
api_key_in:
- header
api_specs:
- filename: vidmob-media-api-openapi.yml
  format: yaml
  label: VidMob Media API
  slug: vidmob-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-media-api-openapi.yml
- filename: vidmob-organization-api-openapi.yml
  format: yaml
  label: VidMob Organization API
  slug: vidmob-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-organization-api-openapi.yml
- filename: vidmob-scoring-api-openapi.yml
  format: yaml
  label: VidMob Scoring API
  slug: vidmob-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-scoring-api-openapi.yml
- filename: vidmob-workspaces-api-openapi.yml
  format: yaml
  label: VidMob Workspaces API
  slug: vidmob-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/openapi/vidmob-workspaces-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Vidmob Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
- jwtBearer
overview: VidMob secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, refreshToken, and jwtBearer flow(s).
provider_name: VidMob
provider_slug: vidmob
scheme_count: 2
schemes:
- docs: https://vidmob-api-docs.readme.io/docs/authentication
  in: header
  name: sec0
  notes: 'The published specs declare the scheme as apiKey in the Authorization header with x-bearer-format bearer, and the docs show the literal header `Authorization: Bearer <api-key>`. Keys are issued per organization by an Organizational Admin at https://acs.vidmob.com/api-key-management and carry capability-domain scopes (see scopes/vidmob-scopes.yml). A key has a name, an expiration and an owning organization, readable via GET /v1/permission.'
  parameter: Authorization
  scheme: Bearer
  sources:
  - openapi/vidmob-creative-aperture-openapi.json
  - openapi/vidmob-creative-scoring-openapi.json
  - openapi/vidmob-public-api-openapi.json
  surface: rest
  type: apiKey
- client_id_metadata_document_supported: false
  dynamic_client_registration:
    endpoint: https://mcp-auth.vidmob.com/v1/oauth2/register
    spec: RFC 7591
    supported: true
  flows:
  - authorizationUrl: https://acs.vidmob.com/oauth/authorize
    flow: authorizationCode
    pkce: S256
    scopes: 5
    tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token
  - flow: refreshToken
    tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token
  - flow: jwtBearer
    grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer
    tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token
  id_token_signing_alg:
  - RS256
  issuer: https://mcp-auth.vidmob.com
  jwks_uri: https://mcp-auth.vidmob.com/.well-known/jwks.json
  name: vidmob-mcp-oauth
  notes: Users authenticate through Vidmob's own login — password or SSO, including 2FA — which then issues the OAuth tokens. Tokens are audience-bound and carry an organization_id claim chosen at authorization (an org picker when the user belongs to several), re-stamped on refresh. Tools never accept an organization identifier as a parameter. The MCP server validates tokens against the published JWKS and does not forward the partner token to backend services.
  sources:
  - https://mcp-auth.vidmob.com/.well-known/oauth-authorization-server
  surface: mcp
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  userinfo_endpoint: https://mcp-auth.vidmob.com/v1/oauth2/userinfo
slug: vidmob-authentication
source_filename: vidmob-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: searched\nsource: openapi/vidmob-creative-aperture-openapi.json, openapi/vidmob-creative-scoring-openapi.json,\n  openapi/vidmob-public-api-openapi.json\ndocs:\n  - https://vidmob-api-docs.readme.io/docs/authentication\n  - https://help.vidmob.com/en/articles/15465541-setting-up-the-vidmob-mcp-connector\n  - https://help.vidmob.com/en/articles/15461399-vidmob-mcp-security-compliance-overview\nsummary:\n  types:\n    - apiKey\n    - oauth2\n  api_key_in:\n    - header\n  oauth2_flows:\n    - authorizationCode\n    - refreshToken\n    - jwtBearer\n  surfaces:\n    rest: apiKey (Bearer) only\n    mcp: oauth2 authorization_code + PKCE, or the same per-organization apiKey\nschemes:\n  - name: sec0\n    type: apiKey\n    in: header\n    parameter: Authorization\n    scheme: Bearer\n    surface: rest\n    sources:\n      - openapi/vidmob-creative-aperture-openapi.json\n      - openapi/vidmob-creative-scoring-openapi.json\n      - openapi/vidmob-public-api-openapi.json\n\
  \    docs: https://vidmob-api-docs.readme.io/docs/authentication\n    notes: >-\n      The published specs declare the scheme as apiKey in the Authorization header with x-bearer-format bearer, and the\n      docs show the literal header `Authorization: Bearer <api-key>`. Keys are issued per organization by an\n      Organizational Admin at https://acs.vidmob.com/api-key-management and carry capability-domain scopes (see\n      scopes/vidmob-scopes.yml). A key has a name, an expiration and an owning organization, readable via\n      GET /v1/permission.\n  - name: vidmob-mcp-oauth\n    type: oauth2\n    surface: mcp\n    sources:\n      - https://mcp-auth.vidmob.com/.well-known/oauth-authorization-server\n    issuer: https://mcp-auth.vidmob.com\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://acs.vidmob.com/oauth/authorize\n        tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token\n        pkce: S256\n        scopes: 5\n      - flow: refreshToken\n    \
  \    tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token\n      - flow: jwtBearer\n        grant_type: urn:ietf:params:oauth:grant-type:jwt-bearer\n        tokenUrl: https://mcp-auth.vidmob.com/v1/oauth2/token\n    dynamic_client_registration:\n      supported: true\n      spec: RFC 7591\n      endpoint: https://mcp-auth.vidmob.com/v1/oauth2/register\n    client_id_metadata_document_supported: false\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - none\n    jwks_uri: https://mcp-auth.vidmob.com/.well-known/jwks.json\n    userinfo_endpoint: https://mcp-auth.vidmob.com/v1/oauth2/userinfo\n    id_token_signing_alg:\n      - RS256\n    notes: >-\n      Users authenticate through Vidmob's own login — password or SSO, including 2FA — which then issues the OAuth\n      tokens. Tokens are audience-bound and carry an organization_id claim chosen at authorization (an org picker when\n      the user belongs to several), re-stamped on refresh. Tools\
  \ never accept an organization identifier as a\n      parameter. The MCP server validates tokens against the published JWKS and does not forward the partner token to\n      backend services.\nsso:\n  supported: true\n  protocol: SAML 2.0\n  mfa: true\n  docs: https://help.vidmob.com/en/articles/7839806-how-do-i-configure-single-sign-on-sso-for-my-organization\nunscoped_endpoints:\n  note: Require a valid API key but no specific scope.\n  operations:\n    - GET /v1/organization\n    - GET /v1/permission\n    - GET /v1/workspaces\nx-evidence:\n  - fetched: '2026-08-05'\n    url: https://vidmob-api-docs.readme.io/docs/authentication.md\n    http_status: 200\n  - fetched: '2026-08-05'\n    url: https://mcp.vidmob.com/mcp\n    http_status: 401\n    note: WWW-Authenticate Bearer resource_metadata challenge — confirms the RFC 9728 discovery chain\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vidmob/refs/heads/main/authentication/vidmob-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- creative-intelligence
- creative-data
- Advertising
- Marketing
- media-measurement
- Video
- computer-vision
- creative-analytics
- adtech
- MCP
- agent-native
- martech
---
