---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ledgerbotje-nl-app-api-openapi.yml
  format: yaml
  label: Ledger Botje App API
  slug: ledgerbotje-nl-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgerbotje-nl/openapi/ledgerbotje-nl-app-api-openapi.yml
- filename: ledgerbotje-nl-well-known-api-openapi.yml
  format: yaml
  label: Ledger Botje .well Known API
  slug: ledgerbotje-nl-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ledgerbotje-nl/openapi/ledgerbotje-nl-well-known-api-openapi.yml
auth_types: []
description: Authentication OAuth 2.1 with PKCE
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ledger Botje Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ledger Botje declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ledger Botje
provider_slug: ledgerbotje-nl
scheme_count: 2
schemes:
- authorize_url: https://ledgerbotje.nl/app/mcp/oauth/authorize
  evidence: Authentication OAuth 2.1 with PKCE
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Log in with your Exact Online account (as described in the connector setup steps).
  name: OAuth 2.1 with PKCE
  scopes:
  - mcp:tools
  type: oauth2
- evidence: 'bearer_methods_supported": ["header"]'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
slug: ledgerbotje-nl-authentication
source_filename: ledgerbotje-nl-authentication.yml
source_heading: Authentication Profile
source_url: https://ledgerbotje.nl/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ledgerbotje.nl/.well-known/oauth-protected-resource\nsources:\n- https://ledgerbotje.nl/.well-known/oauth-protected-resource\n- https://ledgerbotje.nl/.well-known/oauth-authorization-server\n- https://ledgerbotje.nl/en/mcp-koppelen\ndescription: Authentication OAuth 2.1 with PKCE\nschemes:\n- type: oauth2\n  name: OAuth 2.1 with PKCE\n  evidence: Authentication OAuth 2.1 with PKCE\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://ledgerbotje.nl/app/mcp/oauth/authorize\n  scopes:\n  - mcp:tools\n  how_to_obtain: Log in with your Exact Online account (as described in the connector setup steps).\n- type: http-bearer\n  name: Bearer token\n  evidence: 'bearer_methods_supported\": [\"header\"]'\n  location: header\n  header: Authorization\ndocs: https://ledgerbotje.nl/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/ledgerbotje-nl/authentication/ledgerbotje-nl-authentication.yml
summary_line: 2 schemes
tags:
- Accounting
- Artificial Intelligence
- Automation
- ExactOnline
- Netherlands
---
