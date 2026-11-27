---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tabfleet-com-health-api-openapi.yml
  format: yaml
  label: Tabfleet Health API
  slug: tabfleet-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tabfleet-com/openapi/tabfleet-com-health-api-openapi.yml
- filename: tabfleet-com-sessions-api-openapi.yml
  format: yaml
  label: Tabfleet Sessions API
  slug: tabfleet-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tabfleet-com/openapi/tabfleet-com-sessions-api-openapi.yml
- filename: tabfleet-com-usage-api-openapi.yml
  format: yaml
  label: Tabfleet Usage API
  slug: tabfleet-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tabfleet-com/openapi/tabfleet-com-usage-api-openapi.yml
- filename: tabfleet-com-viewer-settings-api-openapi.yml
  format: yaml
  label: Tabfleet Viewer Settings API
  slug: tabfleet-com-viewer-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tabfleet-com/openapi/tabfleet-com-viewer-settings-api-openapi.yml
auth_types: []
description: Authentication methods published by Tabfleet
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Tabfleet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tabfleet declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Tabfleet
provider_slug: tabfleet-com
scheme_count: 2
schemes:
- authorize_url: https://api.tabfleet.com/oauth/authorize
  evidence: Tabfleet supports OAuth authorization code with S256 PKCE for its remote MCP server.
  flows:
  - authorization_code
  how_to_obtain: Register a client (dynamic registration optional) and perform the authorization code flow with S256 PKCE as described in the documentation.
  name: Tabfleet OAuth
  scopes:
  - browser:read
  - browser:control
  - offline_access
  type: oauth2
- evidence: 'Use `Authorization: Bearer YOUR_TABFLEET_API_KEY`.'
  header: Authorization
  how_to_obtain: Create an API key in the Tabfleet dashboard under API keys and store it securely.
  location: header
  name: Tabfleet API key
  type: http-bearer
slug: tabfleet-com-authentication
source_filename: tabfleet-com-authentication.yml
source_heading: Authentication Profile
source_url: https://tabfleet.com/auth.md
source_yaml: "generated: '2026-11-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tabfleet.com/auth.md\nsources:\n- https://tabfleet.com/auth.md\n- https://tabfleet.com/docs/authentication\n- https://tabfleet.com/docs/mcp\n- https://tabfleet.com/docs/quickstart\ndescription: Authentication methods published by Tabfleet\nschemes:\n- type: oauth2\n  name: Tabfleet OAuth\n  evidence: Tabfleet supports OAuth authorization code with S256 PKCE for its remote MCP server.\n  flows:\n  - authorization_code\n  authorize_url: https://api.tabfleet.com/oauth/authorize\n  scopes:\n  - browser:read\n  - browser:control\n  - offline_access\n  how_to_obtain: Register a client (dynamic registration optional) and perform the authorization code flow with S256 PKCE as described in the\n    documentation.\n- type: http-bearer\n  name: Tabfleet API key\n  evidence: 'Use `Authorization: Bearer YOUR_TABFLEET_API_KEY`.'\n  location: header\n  header: Authorization\n  how_to_obtain:\
  \ Create an API key in the Tabfleet dashboard under API keys and store it securely.\ndocs: https://tabfleet.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/tabfleet-com/authentication/tabfleet-com-authentication.yml
summary_line: 2 schemes
tags:
- Cloud
- Browser
- AI
- Infrastructure
- MCP
---
