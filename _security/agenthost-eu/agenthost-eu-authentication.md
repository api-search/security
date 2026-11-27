---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agenthost-eu-openapi-generated.yml
  format: yaml
  label: agenthost API
  slug: agenthost-eu-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agenthost-eu/openapi/_ae-authored/agenthost-eu-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: agenthost Authentication
name_suffix: Authentication
oauth_flows: []
overview: agenthost declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: agenthost
provider_slug: agenthost-eu
scheme_count: 1
schemes:
- description: OAuth 2.1 authorization server with PKCE (S256) and token revocation. Supports authorization code flow.
  flows:
    authorizationCode:
      authorizationUrl: https://agenthost.eu/oauth/authorize
      refreshUrl: https://agenthost.eu/oauth/token
      scopes: {}
      tokenUrl: https://agenthost.eu/oauth/token
  pkce: required
  type: oauth2
slug: agenthost-eu-authentication
source_filename: agenthost-eu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://agenthost.eu/docs/signing-in\nschemes:\n  - type: oauth2\n    description: \"OAuth 2.1 authorization server with PKCE (S256) and token revocation. Supports authorization code flow.\"\n    flows:\n      authorizationCode:\n        authorizationUrl: \"https://agenthost.eu/oauth/authorize\"\n        tokenUrl: \"https://agenthost.eu/oauth/token\"\n        refreshUrl: \"https://agenthost.eu/oauth/token\"\n        scopes: {}\n    pkce: required"
source_yaml_url: https://artifacts.apis.io/agenthost-eu/authentication/agenthost-eu-authentication.yml
summary_line: 1 scheme
tags:
- Web Hosting
- Artificial Intelligence
- MCP
- Cloud
- EU
---
