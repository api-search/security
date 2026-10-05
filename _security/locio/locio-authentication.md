---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Locio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Locio declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Locio
provider_slug: locio
scheme_count: 1
schemes:
- authorize_url: https://locio.com.au/account/authorize
  evidence: '"grant_types_supported":["authorization_code"]'
  flows:
  - authorization_code
  name: OAuth 2.0
  scopes:
  - addresses
  type: oauth2
slug: locio-authentication
source_filename: locio-authentication.yml
source_heading: Authentication Profile
source_url: https://api.locio.com.au/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.locio.com.au/.well-known/oauth-authorization-server\nsources:\n- https://api.locio.com.au/.well-known/oauth-authorization-server\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: '\"grant_types_supported\":[\"authorization_code\"]'\n  flows:\n  - authorization_code\n  authorize_url: https://locio.com.au/account/authorize\n  scopes:\n  - addresses\ndocs: https://api.locio.com.au/.well-known/oauth-authorization-server\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/locio/refs/heads/main/authentication/locio-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Address
- Geocoding
- MCP
---
