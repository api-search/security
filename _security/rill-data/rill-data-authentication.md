---
api_key_in:
- header
api_specs:
- filename: rill-data-admin-openapi.yaml
  format: yaml
  label: Rill Admin API
  slug: rill-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rill-data/refs/heads/main/openapi/rill-data-admin-openapi.yaml
auth_types:
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Rill Data Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- deviceCode
overview: Rill Data secures its APIs with http-bearer and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and deviceCode flow(s).
provider_name: Rill Data
provider_slug: rill-data
scheme_count: 2
schemes:
- format: 'Authorization: Bearer <token>'
  header: Authorization
  location: header
  name: bearerToken
  scheme: bearer
  sources:
  - https://docs.rilldata.com/guide/administration/access-tokens/user-tokens
  token_types:
  - description: Personal access token tied to an individual user account; inherits the user's org role (admin/editor/viewer/guest) and project roles (admin/editor/viewer). Issued via `rill token issue`.
    kind: user-token
    management:
    - rill token issue
    - rill token list
    - rill token revoke
  - description: Organization-scoped token for programmatic/automated (non-user) access.
    kind: service-token
  type: http
- authorization_endpoint: https://admin.rilldata.com/auth/oauth/authorize
  description: OAuth 2.1 authorization-code flow with PKCE used by the hosted Rill MCP server and OAuth-based connectors. Advertised via RFC 8414 metadata at https://api.rilldata.com/.well-known/oauth-authorization-server.
  grant_types:
  - authorization_code
  - urn:ietf:params:oauth:grant-type:device_code
  - refresh_token
  jwks_uri: https://admin.rilldata.com/.well-known/jwks.json
  name: oauth2
  pkce: S256
  registration_endpoint: https://admin.rilldata.com/auth/oauth/register
  scopes:
  - offline_access
  sources:
  - well-known/rill-data-oauth-authorization-server.json
  token_endpoint: https://admin.rilldata.com/auth/oauth/token
  type: oauth2
slug: rill-data-authentication
source_filename: rill-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.rilldata.com/guide/administration/access-tokens/user-tokens\ndocs: https://docs.rilldata.com/guide/administration/access-tokens/user-tokens\nsummary:\n  types: [http-bearer, oauth2]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, deviceCode]\nschemes:\n  - name: bearerToken\n    type: http\n    scheme: bearer\n    location: header\n    header: Authorization\n    format: \"Authorization: Bearer <token>\"\n    token_types:\n      - kind: user-token\n        description: >-\n          Personal access token tied to an individual user account; inherits the\n          user's org role (admin/editor/viewer/guest) and project roles\n          (admin/editor/viewer). Issued via `rill token issue`.\n        management: [rill token issue, rill token list, rill token revoke]\n      - kind: service-token\n        description: Organization-scoped token for programmatic/automated (non-user) access.\n    sources: [https://docs.rilldata.com/guide/administration/access-tokens/user-tokens]\n\
  \  - name: oauth2\n    type: oauth2\n    description: >-\n      OAuth 2.1 authorization-code flow with PKCE used by the hosted Rill MCP\n      server and OAuth-based connectors. Advertised via RFC 8414 metadata at\n      https://api.rilldata.com/.well-known/oauth-authorization-server.\n    authorization_endpoint: https://admin.rilldata.com/auth/oauth/authorize\n    token_endpoint: https://admin.rilldata.com/auth/oauth/token\n    registration_endpoint: https://admin.rilldata.com/auth/oauth/register\n    jwks_uri: https://admin.rilldata.com/.well-known/jwks.json\n    grant_types: [authorization_code, \"urn:ietf:params:oauth:grant-type:device_code\", refresh_token]\n    pkce: S256\n    scopes: [offline_access]\n    sources: [well-known/rill-data-oauth-authorization-server.json]\npermissions_model: >-\n  Rill uses role-based access (admin/editor/viewer/guest at the org level;\n  admin/editor/viewer at the project level) plus attribute-based security\n  policies (email, domain, groups). The\
  \ admin REST API has no per-request OAuth\n  scope surface beyond the token's inherited roles.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rill-data/refs/heads/main/authentication/rill-data-authentication.yml
summary_line: http-bearer/oauth2 · 2 schemes
tags:
- Company
- Analytics
- Business Intelligence
- Dashboards
- Metrics
- Data
- OLAP
- Open Source
- Developer Tools
---
