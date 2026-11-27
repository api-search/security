---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mdedit-ai-openapi-generated.yml
  format: yaml
  label: mdedit.ai API
  slug: mdedit-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mdedit-ai/openapi/_ae-authored/mdedit-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for mdedit.ai
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: mdedit.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: mdedit.ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mdedit.ai
provider_slug: mdedit-ai
scheme_count: 1
schemes:
- evidence: For clients without browser sign-in, CI, or unattended workflows, create a scoped key in Settings → Integrations → API Keys .
  header: X-API-Key
  how_to_obtain: Create an API key in Settings → Integrations → API Keys in the mdedit.ai web UI (or via the POST /api-keys endpoint for scoped keys).
  location: header
  name: API Key
  type: apiKey
slug: mdedit-ai-authentication
source_filename: mdedit-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://mdedit.ai/docs/agents/mcp-authentication
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mdedit.ai/docs/agents/mcp-authentication\nsources:\n- https://mdedit.ai/docs/agents/mcp-authentication\n- https://mdedit.ai/docs/api-keys\n- https://mdedit.ai/docs/getting-started\ndescription: Authentication methods for mdedit.ai\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: For clients without browser sign-in, CI, or unattended workflows, create a scoped key in Settings → Integrations → API Keys .\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key in Settings → Integrations → API Keys in the mdedit.ai web UI (or via the POST /api-keys endpoint for scoped\n    keys).\ndocs: https://mdedit.ai/docs/agents/mcp-authentication\n"
source_yaml_url: https://artifacts.apis.io/mdedit-ai/authentication/mdedit-ai-authentication.yml
summary_line: 1 scheme
tags:
- Markdown editor
- Technical Writing
- Documentation
- AI Assistance
- Collaboration
- Offline-First
- Publishing
- Developer Tools
---
