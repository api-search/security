---
anonymous_access: false
api_key_in: []
api_specs:
- filename: krosyn-connectors-api-openapi.yml
  format: yaml
  label: Chmura Software Connectors API
  slug: krosyn-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/krosyn/refs/heads/main/openapi/krosyn-connectors-api-openapi.yml
auth_types: []
description: Authentication methods for Krosyn REST API and MCP server
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Krosyn Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chmura Software declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Chmura Software
provider_slug: krosyn
scheme_count: 2
schemes:
- evidence: 'Include your token in the Authorization header as a Bearer token: Authorization: Bearer your-api-token-here'
  header: Authorization
  how_to_obtain: Create a token in Settings > API Tokens in the Krosyn dashboard.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: OAuth 2.1 -- for MCP clients (AI tools). The client connects with just the server URL, and the authorization flow happens in your browser.
  name: OAuth 2.1
  type: oauth2
slug: krosyn-authentication
source_filename: krosyn-authentication.yml
source_heading: Authentication Profile
source_url: https://krosyn.com/docs/api-authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://krosyn.com/docs/api-authentication\nsources:\n- https://krosyn.com/docs/api-authentication\n- https://krosyn.com/docs\ndescription: Authentication methods for Krosyn REST API and MCP server\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Include your token in the Authorization header as a Bearer token: Authorization: Bearer your-api-token-here'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token in Settings > API Tokens in the Krosyn dashboard.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: OAuth 2.1 -- for MCP clients (AI tools). The client connects with just the server URL, and the authorization flow happens in your\n    browser.\ndocs: https://krosyn.com/docs/api-authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/krosyn/refs/heads/main/authentication/krosyn-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Cloud
- API
- DeveloperTools
- Security
---
