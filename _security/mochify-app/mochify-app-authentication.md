---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mochify-app-generate-api-openapi.yml
  format: yaml
  label: mochify-app Generate API
  slug: mochify-app-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mochify-app/openapi/mochify-app-generate-api-openapi.yml
- filename: mochify-app-image-api-openapi.yml
  format: yaml
  label: mochify-app Image API
  slug: mochify-app-image-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mochify-app/openapi/mochify-app-image-api-openapi.yml
- filename: mochify-app-meta-api-openapi.yml
  format: yaml
  label: mochify-app Meta API
  slug: mochify-app-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mochify-app/openapi/mochify-app-meta-api-openapi.yml
- filename: mochify-app-pdf-api-openapi.yml
  format: yaml
  label: mochify-app PDF API
  slug: mochify-app-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mochify-app/openapi/mochify-app-pdf-api-openapi.yml
- filename: mochify-app-upload-api-openapi.yml
  format: yaml
  label: mochify-app Upload API
  slug: mochify-app-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mochify-app/openapi/mochify-app-upload-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mochify App Authentication
name_suffix: Authentication
oauth_flows: []
overview: mochify-app declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mochify-app
provider_slug: mochify-app
scheme_count: 1
schemes:
- authorize_url: https://mcp.mochify.app/oauth/authorize
  evidence: '"authorization_endpoint":"https://mcp.mochify.app/oauth/authorize"'
  flows:
  - authorization_code
  name: OAuth2
  scopes:
  - squish
  token_url: https://mcp.mochify.app/oauth/token
  type: oauth2
slug: mochify-app-authentication
source_filename: mochify-app-authentication.yml
source_heading: Authentication Profile
source_url: https://mcp.mochify.app/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mcp.mochify.app/.well-known/oauth-authorization-server\nsources:\n- https://mcp.mochify.app/.well-known/oauth-authorization-server\nschemes:\n- type: oauth2\n  name: OAuth2\n  evidence: '\"authorization_endpoint\":\"https://mcp.mochify.app/oauth/authorize\"'\n  flows:\n  - authorization_code\n  token_url: https://mcp.mochify.app/oauth/token\n  authorize_url: https://mcp.mochify.app/oauth/authorize\n  scopes:\n  - squish\ndocs: https://mcp.mochify.app/.well-known/oauth-authorization-server\n"
source_yaml_url: https://artifacts.apis.io/mochify-app/authentication/mochify-app-authentication.yml
summary_line: 1 scheme
tags:
- Company
- ImageCompression
- VideoCompression
- PDFCompression
- AI
- PrivacyFocused
---
