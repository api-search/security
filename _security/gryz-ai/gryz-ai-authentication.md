---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gryz-ai-openapi-generated.yml
  format: yaml
  label: Gryz API
  slug: gryz-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gryz-ai/openapi/_ae-authored/gryz-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for Gryz MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Gryz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gryz declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Gryz
provider_slug: gryz-ai
scheme_count: 2
schemes:
- evidence: Complete OAuth sign‑in when prompted. Your browser opens to authorize access
  how_to_obtain: Complete OAuth sign‑in when prompted; your browser opens to authorize access.
  name: OAuth
  type: oauth2
- evidence: Generate a key on the API keys page , then add it as a Bearer token
  header: Authorization
  how_to_obtain: Generate a key on the API keys page, then add it as a Bearer token.
  location: header
  name: Bearer token
  type: http-bearer
slug: gryz-ai-authentication
source_filename: gryz-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.gryz.ai/docs/mcp/setup/
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.gryz.ai/docs/mcp/setup/\nsources:\n- https://www.gryz.ai/docs/mcp/setup/\n- https://www.gryz.ai/docs/getting-started/agents/\n- https://www.gryz.ai/docs/getting-started/publish-first-document/\n- https://www.gryz.ai/docs/getting-started/create-account/\ndescription: Authentication methods for Gryz MCP\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Complete OAuth sign‑in when prompted. Your browser opens to authorize access\n  how_to_obtain: Complete OAuth sign‑in when prompted; your browser opens to authorize access.\n- type: http-bearer\n  name: Bearer token\n  evidence: Generate a key on the API keys page , then add it as a Bearer token\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a key on the API keys page, then add it as a Bearer token.\ndocs: https://www.gryz.ai/docs/mcp/setup/\n"
source_yaml_url: https://artifacts.apis.io/gryz-ai/authentication/gryz-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Collaboration
- Context
- Memory
- Shared
---
