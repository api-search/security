---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Creadal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Creadal declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Creadal
provider_slug: creadal-com
scheme_count: 3
schemes:
- applies_to: https://creadal.com/mcp
  authorization_url: https://creadal.com/oauth/authorize
  dynamic_client_registration: true
  evidence: https://creadal.com/.well-known/oauth-authorization-server (HTTP 200) and https://creadal.com/.well-known/oauth-protected-resource (HTTP 200, bearer_methods_supported [header])
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  name: oauth2
  pkce: S256
  registration_url: https://creadal.com/oauth/register
  revocation_url: https://creadal.com/oauth/revoke
  scopes:
  - designs:create
  - designs:read
  - quota:read
  token_endpoint_auth_methods:
  - none
  token_url: https://creadal.com/oauth/token
  type: oauth2
- applies_to: https://creadal.com/mcp
  description: Developers can also call it with a workspace API key (Bearer token), made under Settings in Creadal.
  name: workspace-api-key
  scheme: bearer
  type: http
- description: list_packaging_models and generate_dieline are documented as "Free, no sign-in."
  name: anonymous
  type: none
slug: creadal-com-authentication
source_filename: creadal-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://creadal.com/mcp-server/\ndocs: https://creadal.com/mcp-server/\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  authorization_url: https://creadal.com/oauth/authorize\n  token_url: https://creadal.com/oauth/token\n  revocation_url: https://creadal.com/oauth/revoke\n  registration_url: https://creadal.com/oauth/register\n  dynamic_client_registration: true\n  token_endpoint_auth_methods: [none]\n  grant_types: [authorization_code, refresh_token]\n  scopes: [designs:create, designs:read, quota:read]\n  applies_to: https://creadal.com/mcp\n  evidence: https://creadal.com/.well-known/oauth-authorization-server (HTTP 200) and https://creadal.com/.well-known/oauth-protected-resource (HTTP 200, bearer_methods_supported [header])\n- name: workspace-api-key\n  type: http\n  scheme: bearer\n  description: \"Developers can also call it with a workspace API key (Bearer token), made under Settings\
  \ in Creadal.\"\n  applies_to: https://creadal.com/mcp\n- name: anonymous\n  type: none\n  description: \"list_packaging_models and generate_dieline are documented as \\\"Free, no sign-in.\\\"\"\nnote: Creadal publishes no REST API; authentication applies to its remote MCP server. Metadata documents were read with GET only; no OAuth or token endpoint was called.\n"
source_yaml_url: https://artifacts.apis.io/creadal-com/authentication/creadal-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Design
- Templates
- Packaging
- Mockups
- Dielines
- MCP
- Graphic Design
---
