---
anonymous_access: false
api_key_in: []
api_specs:
- filename: naia-today-v1-openapi.json
  format: json
  label: naia API V1 API
  slug: naia-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/naia-today/openapi/_original/naia-today-v1-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Naia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Naia declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Naia
provider_slug: naia-today
scheme_count: 2
schemes:
- authorize_url: https://naia.today/api/oauth/mcp/authorize
  evidence: '"authorization_endpoint":"https://naia.today/api/oauth/mcp/authorize"'
  flows:
  - authorization_code
  - client_credentials
  - refresh_token
  name: OAuth2
  scopes:
  - openid
  - profile
  - email
  - offline_access
  type: oauth2
- evidence: '"bearer_methods_supported":["header"]'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: naia-today-authentication
source_filename: naia-today-authentication.yml
source_heading: Authentication Profile
source_url: https://naia.today/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://naia.today/.well-known/oauth-authorization-server\nsources:\n- https://naia.today/.well-known/oauth-authorization-server\n- https://naia.today/.well-known/oauth-protected-resource\n- https://naia.today/.well-known/mcp-registry-auth\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: '\"authorization_endpoint\":\"https://naia.today/api/oauth/mcp/authorize\"'\n  flows:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  authorize_url: https://naia.today/api/oauth/mcp/authorize\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n- type: http-bearer\n  name: Bearer\n  evidence: '\"bearer_methods_supported\":[\"header\"]'\n  location: header\n  header: Authorization\ndocs: https://naia.today/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/naia-today/authentication/naia-today-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- SEO
- Geo
- Content
- Marketing
---
