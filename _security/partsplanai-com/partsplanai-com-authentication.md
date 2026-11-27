---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for PartsPlan AI MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: PartsPlan AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: PartsPlan AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: PartsPlan AI
provider_slug: partsplanai-com
scheme_count: 2
schemes:
- evidence: 'Send it as Authorization: Bearer <key> or x-api-key: <key>.'
  header: Authorization
  how_to_obtain: Create an API key under 'My MCP keys' after signing in; the key starts with pk_live_ and is shown only once.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'Send it as Authorization: Bearer <key> or x-api-key: <key>.'
  header: x-api-key
  how_to_obtain: Create an API key under 'My MCP keys' after signing in; the key starts with pk_live_ and is shown only once.
  location: header
  name: API key header
  type: apiKey
slug: partsplanai-com-authentication
source_filename: partsplanai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://partsplanai.com/en/developers
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://partsplanai.com/en/developers\nsources:\n- https://partsplanai.com/en/developers\ndescription: Authentication methods for PartsPlan AI MCP\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send it as Authorization: Bearer <key> or x-api-key: <key>.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key under 'My MCP keys' after signing in; the key starts with pk_live_ and is shown only once.\n- type: apiKey\n  name: API key header\n  evidence: 'Send it as Authorization: Bearer <key> or x-api-key: <key>.'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create an API key under 'My MCP keys' after signing in; the key starts with pk_live_ and is shown only once.\ndocs: https://partsplanai.com/en/developers\n"
source_yaml_url: https://artifacts.apis.io/partsplanai-com/authentication/partsplanai-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Datasheets
- Electronics
- Verification
- Seoul
---
