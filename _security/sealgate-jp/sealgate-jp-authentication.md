---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sealgate-jp-openapi-generated.yml
  format: yaml
  label: sealgate-jp API
  slug: sealgate-jp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sealgate-jp/openapi/_ae-authored/sealgate-jp-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sealgate Jp Authentication
name_suffix: Authentication
oauth_flows: []
overview: sealgate-jp declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: sealgate-jp
provider_slug: sealgate-jp
scheme_count: 1
schemes:
- authorizationUrl: https://api.sealgate.jp/v1/oauth/authorize
  description: OAuth 2.1 dynamic client registration with PKCE S256 for MCP and API access
  flow: authorizationCode
  tokenUrl: https://api.sealgate.jp/v1/oauth/token
  type: oauth2
slug: sealgate-jp-authentication
source_filename: sealgate-jp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://sealgate.jp/docs#authentication\nschemes:\n  - type: oauth2\n    flow: authorizationCode\n    description: OAuth 2.1 dynamic client registration with PKCE S256 for MCP and API access\n    tokenUrl: https://api.sealgate.jp/v1/oauth/token\n    authorizationUrl: https://api.sealgate.jp/v1/oauth/authorize\n"
source_yaml_url: https://artifacts.apis.io/sealgate-jp/authentication/sealgate-jp-authentication.yml
summary_line: 1 scheme
tags:
- Authentication
- WebAuthn
- FIDO2
- Security
- Japan
---
