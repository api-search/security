---
anonymous_access: false
api_key_in: []
api_specs:
- filename: busyboard-app-api-openapi.yml
  format: yaml
  label: BusyBoard API API
  slug: busyboard-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/busyboard-app/openapi/_original/busyboard-app-api-openapi.yml
auth_types: []
description: Authentication for BusyBoard MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Busyboard App Authentication
name_suffix: Authentication
oauth_flows: []
overview: BusyBoard declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BusyBoard
provider_slug: busyboard-app
scheme_count: 1
schemes:
- evidence: 'Paste this into the assistant''s MCP config with your key: { "mcpServers": { "busyboard": { "url": "https://busyboard.app/api/mcp", "headers": { "Authorization": "Bearer bb_live_your_key_here" } } } }'
  header: Authorization
  how_to_obtain: Create an API key in BusyBoard Settings → API and copy the key that starts with bb_live_
  location: header
  name: Bearer
  type: http-bearer
slug: busyboard-app-authentication
source_filename: busyboard-app-authentication.yml
source_heading: Authentication Profile
source_url: https://busyboard.app/guides/let-your-ai-assistant-manage-your-availability
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://busyboard.app/guides/let-your-ai-assistant-manage-your-availability\nsources:\n- https://busyboard.app/guides/let-your-ai-assistant-manage-your-availability\ndescription: Authentication for BusyBoard MCP API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Paste this into the assistant''s MCP config with your key: { \"mcpServers\": { \"busyboard\": { \"url\": \"https://busyboard.app/api/mcp\",\n    \"headers\": { \"Authorization\": \"Bearer bb_live_your_key_here\" } } } }'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in BusyBoard Settings → API and copy the key that starts with bb_live_\ndocs: https://busyboard.app/guides/let-your-ai-assistant-manage-your-availability\n"
source_yaml_url: https://artifacts.apis.io/busyboard-app/authentication/busyboard-app-authentication.yml
summary_line: 1 scheme
tags:
- Scheduling
- Calendar
- Privacy
- Free
- Software-as-a-Service
---
