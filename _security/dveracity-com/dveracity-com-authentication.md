---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dveracity-com-openapi-generated.yml
  format: yaml
  label: dVeracity API
  slug: dveracity-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dveracity-com/openapi/_ae-authored/dveracity-com-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: dVeracity Authentication
name_suffix: Authentication
oauth_flows: []
overview: dVeracity declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: dVeracity
provider_slug: dveracity-com
scheme_count: 1
schemes:
- authorize_url: https://api.dveracity.com/authorize
  evidence: '"authorization_endpoint":"https://api.dveracity.com/authorize"'
  flows:
  - authorization_code
  name: OAuth 2.0
  scopes:
  - semantic:query
  - semantic:templates
  - ofp:read
  - ofp:validate
  - compliance:read
  - compliance:evaluate
  - offline_access
  token_url: https://api.dveracity.com/token
  type: oauth2
slug: dveracity-com-authentication
source_filename: dveracity-com-authentication.yml
source_heading: Authentication Profile
source_url: https://api.dveracity.com/.well-known/oauth-protected-resource/mcp
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.dveracity.com/.well-known/oauth-protected-resource/mcp\nsources:\n- https://api.dveracity.com/.well-known/oauth-protected-resource/mcp\n- https://api.dveracity.com/.well-known/oauth-authorization-server\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: '\"authorization_endpoint\":\"https://api.dveracity.com/authorize\"'\n  flows:\n  - authorization_code\n  token_url: https://api.dveracity.com/token\n  authorize_url: https://api.dveracity.com/authorize\n  scopes:\n  - semantic:query\n  - semantic:templates\n  - ofp:read\n  - ofp:validate\n  - compliance:read\n  - compliance:evaluate\n  - offline_access\ndocs: https://api.dveracity.com/.well-known/oauth-protected-resource/mcp\n"
source_yaml_url: https://artifacts.apis.io/dveracity-com/authentication/dveracity-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Emissions
- Verification
- Carbon Accounting
- Open Standard
---
