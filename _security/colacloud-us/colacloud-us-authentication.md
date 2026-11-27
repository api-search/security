---
anonymous_access: false
api_key_in: []
api_specs:
- filename: colacloud-us-colas-api-openapi.yml
  format: yaml
  label: COLA Cloud COLAs API
  slug: colacloud-us-colas-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/colacloud-us/openapi/colacloud-us-colas-api-openapi.yml
auth_types: []
description: Authentication methods for COLA Cloud API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: COLA Cloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: COLA Cloud declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: COLA Cloud
provider_slug: colacloud-us
scheme_count: 2
schemes:
- evidence: 'Self-serve REST, SDK, and CLI requests use a COLA Cloud API key in the `X-API-Key` header:'
  header: X-API-Key
  how_to_obtain: Generate API keys at Dashboard > API Keys in the web app.
  location: header
  name: API Key
  type: apiKey
- evidence: 'MCP clients may use the same key as a Bearer token:'
  header: Authorization
  how_to_obtain: Generate API keys at Dashboard > API Keys in the web app and use the key as a Bearer token.
  location: header
  name: Bearer Token
  type: http-bearer
slug: colacloud-us-authentication
source_filename: colacloud-us-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.colacloud.us/authentication.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.colacloud.us/authentication.md\nsources:\n- https://docs.colacloud.us/authentication.md\n- https://docs.colacloud.us/quickstart.md\n- https://docs.colacloud.us/agent-quickstart.md\n- https://docs.colacloud.us/sdks/mcp-claude.md\ndescription: Authentication methods for COLA Cloud API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Self-serve REST, SDK, and CLI requests use a COLA Cloud API key in the `X-API-Key` header:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Generate API keys at Dashboard > API Keys in the web app.\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'MCP clients may use the same key as a Bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate API keys at Dashboard > API Keys in the web app and use the key as a Bearer token.\nnote: OAuth flows are mentioned for MCP connectors but no token\
  \ or authorize URLs, scopes, or flow details are provided on the pages.\ndocs: https://docs.colacloud.us/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/colacloud-us/authentication/colacloud-us-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data
- Alcohol
- Compliance
- Open Data
---
