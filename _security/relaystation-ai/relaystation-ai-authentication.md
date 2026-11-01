---
anonymous_access: false
api_key_in: []
api_specs:
- filename: relaystation-ai-api-openapi.json
  format: json
  label: Relaystation Api API
  slug: relaystation-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/relaystation-ai/openapi/_original/relaystation-ai-api-openapi.json
auth_types: []
description: Authentication methods as documented
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Relaystation Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: relaystation-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: relaystation-ai
provider_slug: relaystation-ai
scheme_count: 1
schemes:
- evidence: 'Calls: the HTTP API (send the key as Authorization: Bearer rs_live_... ) or an MCP client.'
  header: Authorization
  location: header
  name: API key (rs_live_)
  type: http-bearer
slug: relaystation-ai-authentication
source_filename: relaystation-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://relaystation.ai/docs/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://relaystation.ai/docs/authentication\nsources:\n- https://relaystation.ai/docs/authentication\n- https://relaystation.ai/docs/tokens\n- https://relaystation.ai/docs/tokens.md\n- https://relaystation.ai/docs/quickstart\ndescription: Authentication methods as documented\nschemes:\n- type: http-bearer\n  name: API key (rs_live_)\n  evidence: 'Calls: the HTTP API (send the key as Authorization: Bearer rs_live_... ) or an MCP client.'\n  location: header\n  header: Authorization\nnote: OAuth flow URLs and scopes are not provided on the pages; therefore OAuth details are absent. 1 extracted row(s) were dropped because their\n  quote was not on the page.\ndocs: https://relaystation.ai/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/relaystation-ai/authentication/relaystation-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Data-Relay
- Real-time
- Cloud
---
