---
anonymous_access: false
api_key_in: []
api_specs:
- filename: easydata-cc-openapi-generated.yml
  format: yaml
  label: EasyData API
  slug: easydata-cc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/easydata-cc/openapi/_ae-authored/easydata-cc-openapi-generated.yml
auth_types: []
description: Authentication methods published for EasyData
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: EasyData Authentication
name_suffix: Authentication
oauth_flows: []
overview: EasyData declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: EasyData
provider_slug: easydata-cc
scheme_count: 2
schemes:
- authorize_url: https://easydata.cc/oauth/authorize
  evidence: Start Authorization Code flow at https://easydata.cc/oauth/authorize with response_type=code, an exact registered redirect_uri, state, scope (read or read write), resource, and PKCE S256 challenge.
  flows:
  - authorization_code
  how_to_obtain: Register a public client at https://easydata.cc/api/oauth/register (token_endpoint_auth_method=none), then perform the Authorization Code flow to obtain an access token.
  name: Standard OAuth
  scopes:
  - read
  - write
  type: oauth2
- evidence: 'Send access tokens only in Authorization: Bearer headers.'
  header: Authorization
  how_to_obtain: Obtain an access token via the OAuth Authorization Code flow (or claim grant) and include it in the Authorization header as "Bearer <token>".
  location: header
  name: Bearer token
  type: http-bearer
slug: easydata-cc-authentication
source_filename: easydata-cc-authentication.yml
source_heading: Authentication Profile
source_url: https://easydata.cc/auth.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://easydata.cc/auth.md\nsources:\n- https://easydata.cc/auth.md\n- https://easydata.cc/.well-known/oauth-authorization-server\n- https://easydata.cc/.well-known/oauth-protected-resource/api/public/v1\ndescription: Authentication methods published for EasyData\nschemes:\n- type: oauth2\n  name: Standard OAuth\n  evidence: Start Authorization Code flow at https://easydata.cc/oauth/authorize with response_type=code, an exact registered redirect_uri, state,\n    scope (read or read write), resource, and PKCE S256 challenge.\n  flows:\n  - authorization_code\n  authorize_url: https://easydata.cc/oauth/authorize\n  scopes:\n  - read\n  - write\n  how_to_obtain: Register a public client at https://easydata.cc/api/oauth/register (token_endpoint_auth_method=none), then perform the Authorization\n    Code flow to obtain an access token.\n- type: http-bearer\n  name: Bearer token\n  evidence:\
  \ 'Send access tokens only in Authorization: Bearer headers.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an access token via the OAuth Authorization Code flow (or claim grant) and include it in the Authorization header as \"Bearer\n    <token>\".\ndocs: https://easydata.cc/auth.md\n"
source_yaml_url: https://artifacts.apis.io/easydata-cc/authentication/easydata-cc-authentication.yml
summary_line: 2 schemes
tags:
- Data Management
- Artificial Intelligence
- Spreadsheets
- Collaboration
- Software-as-a-Service
---
