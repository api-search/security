---
anonymous_access: false
api_key_in: []
api_specs:
- filename: etlworks-openapi-generated.yml
  format: yaml
  label: Etlworks API
  slug: etlworks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/etlworks/openapi/_ae-authored/etlworks-openapi-generated.yml
auth_types: []
description: Authentication methods for Etlworks APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Etlworks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Etlworks declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Etlworks
provider_slug: etlworks
scheme_count: 2
schemes:
- evidence: 'Send the key on every request via the Authorization header: HTTP Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: Generate an API key under Settings → Users → Edit → API Key in the Etlworks UI.
  location: header
  name: API key
  type: http-bearer
- evidence: 'For interactive apps, exchange username + password for a short-lived JWT, then send the JWT on subsequent calls. Same Authorization: Bearer … header.'
  header: Authorization
  how_to_obtain: POST to /v1/token-auth/issue with JSON body {"login":"...","password":"..."} to receive a JWT token.
  location: header
  name: Username/password JWT
  token_url: https://app.etlworks.com/rest/v1/token-auth/issue
  type: http-bearer
slug: etlworks-authentication
source_filename: etlworks-authentication.yml
source_heading: Authentication Profile
source_url: https://etlworks.com/dev/api/quickstart.html
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://etlworks.com/dev/api/quickstart.html\nsources:\n- https://etlworks.com/dev/api/quickstart.html\n- https://etlworks.com/dev/ai/quickstart.html\n- https://etlworks.com/dev/ai/mcp.html\ndescription: Authentication methods for Etlworks APIs\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Send the key on every request via the Authorization header: HTTP Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key under Settings → Users → Edit → API Key in the Etlworks UI.\n- type: http-bearer\n  name: Username/password JWT\n  evidence: 'For interactive apps, exchange username + password for a short-lived JWT, then send the JWT on subsequent calls. Same Authorization:\n    Bearer … header.'\n  location: header\n  header: Authorization\n  token_url: https://app.etlworks.com/rest/v1/token-auth/issue\n  how_to_obtain:\
  \ POST to /v1/token-auth/issue with JSON body {\"login\":\"...\",\"password\":\"...\"} to receive a JWT token.\ndocs: https://etlworks.com/dev/api/quickstart.html\n"
source_yaml_url: https://artifacts.apis.io/etlworks/authentication/etlworks-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data Integration
- ETL
- API
- Cloud
---
