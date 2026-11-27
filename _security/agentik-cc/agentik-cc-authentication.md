---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentik-cc-discover-api-openapi.yml
  format: yaml
  label: Agentik Discover API
  slug: agentik-cc-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-discover-api-openapi.yml
- filename: agentik-cc-oauth-api-openapi.yml
  format: yaml
  label: Agentik OAuth API
  slug: agentik-cc-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-oauth-api-openapi.yml
- filename: agentik-cc-run-api-openapi.yml
  format: yaml
  label: Agentik Run API
  slug: agentik-cc-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-run-api-openapi.yml
- filename: agentik-cc-wallet-api-openapi.yml
  format: yaml
  label: Agentik Wallet API
  slug: agentik-cc-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentik-cc/openapi/agentik-cc-wallet-api-openapi.yml
auth_types: []
description: Authentication methods for Agentik
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Agentik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agentik declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Agentik
provider_slug: agentik-cc
scheme_count: 2
schemes:
- evidence: Connect to https://ai.agentik.cc/mcp with OAuth where your client supports it
  name: OAuth
  type: oauth2
- evidence: 'Protected requests use Authorization: Bearer <Agentik API key>'
  header: Authorization
  how_to_obtain: Create, label and revoke keys in the workspace
  location: header
  name: Agentik API key
  type: http-bearer
slug: agentik-cc-authentication
source_filename: agentik-cc-authentication.yml
source_heading: Authentication Profile
source_url: https://www.agentik.cc/ai-agent-tools-without-api-keys.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.agentik.cc/ai-agent-tools-without-api-keys.md\nsources:\n- https://www.agentik.cc/ai-agent-tools-without-api-keys.md\n- https://www.agentik.cc/docs/authentication\n- https://www.agentik.cc/docs/authentication.md\n- https://www.agentik.cc/docs/clients\ndescription: Authentication methods for Agentik\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Connect to https://ai.agentik.cc/mcp with OAuth where your client supports it\n- type: http-bearer\n  name: Agentik API key\n  evidence: 'Protected requests use Authorization: Bearer <Agentik API key>'\n  location: header\n  header: Authorization\n  how_to_obtain: Create, label and revoke keys in the workspace\ndocs: https://www.agentik.cc/ai-agent-tools-without-api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/agentik-cc/authentication/agentik-cc-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Automation
- Tools
- MCP
- Software-as-a-Service
---
