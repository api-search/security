---
anonymous_access: false
api_key_in: []
api_specs:
- filename: daptatech-com-openapi-generated.yml
  format: yaml
  label: Dapta API
  slug: daptatech-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/daptatech-com/openapi/_ae-authored/daptatech-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Dapta MCP and dCal APIs as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Daptatech Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dapta declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Dapta
provider_slug: daptatech-com
scheme_count: 2
schemes:
- evidence: 'Header `x-api-key: <your-key>` (or `Authorization: Bearer <your-key>`) on `https://mcp.dapta.ai/mcp`.'
  header: x-api-key
  how_to_obtain: Create the key in the Dapta admin panel under MCP Access; copy it once shown.
  location: header
  name: x-api-key
  type: apiKey
- evidence: 'Send the key with every request in the `Authorization` header, as `Authorization: Bearer <your key>`.'
  header: Authorization
  how_to_obtain: Create the key in the Dapta admin panel under MCP Access; copy it once shown.
  location: header
  name: Authorization
  type: http-bearer
slug: daptatech-com-authentication
source_filename: daptatech-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.dapta.ai/dapta-mcp/setup/mint-your-api-key.md
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.dapta.ai/dapta-mcp/setup/mint-your-api-key.md\nsources:\n- https://docs.dapta.ai/dapta-mcp/setup/mint-your-api-key.md\n- https://docs.dapta.ai/dforms/developers/api-keys.md\n- https://docs.dapta.ai/dcal/developers/api-keys.md\n- https://docs.dapta.ai/dcal/developers/connect-with-sign-in.md\ndescription: Authentication methods for Dapta MCP and dCal APIs as documented.\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: 'Header `x-api-key: <your-key>` (or `Authorization: Bearer <your-key>`) on `https://mcp.dapta.ai/mcp`.'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create the key in the Dapta admin panel under MCP Access; copy it once shown.\n- type: http-bearer\n  name: Authorization\n  evidence: 'Send the key with every request in the `Authorization` header, as `Authorization: Bearer <your key>`.'\n  location: header\n  header: Authorization\n\
  \  how_to_obtain: Create the key in the Dapta admin panel under MCP Access; copy it once shown.\ndocs: https://docs.dapta.ai/dapta-mcp/setup/mint-your-api-key.md\n"
source_yaml_url: https://artifacts.apis.io/daptatech-com/authentication/daptatech-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- SalesAutomation
- VoiceAgents
- TextAgents
---
