---
anonymous_access: false
api_key_in: []
api_specs:
- filename: chatthing-ai-openapi-generated.yml
  format: yaml
  label: Chat Thing API
  slug: chatthing-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chatthing-ai/openapi/_ae-authored/chatthing-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for Chat Thing MCP
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Chatthing Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chat Thing declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Chat Thing
provider_slug: chatthing-ai
scheme_count: 2
schemes:
- evidence: 'Add it to your client''s MCP config as a bearer token in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Generate an API key on the Connect agent page and copy it.
  location: header
  name: API key
  type: http-bearer
- evidence: Your assistant opens a Chat Thing page, you click **Approve**, and it's issued a token automatically.
  how_to_obtain: Approve the assistant in the browser when it opens the Authorize page.
  name: Browser approval
  type: oauth2
slug: chatthing-ai-authentication
source_filename: chatthing-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://chatthing.ai/docs/mcp/authentication.md
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://chatthing.ai/docs/mcp/authentication.md\nsources:\n- https://chatthing.ai/docs/mcp/authentication.md\n- https://chatthing.ai/docs/mcp/authentication\n- https://chatthing.ai/docs/developers/api-overview\n- https://chatthing.ai/docs/bot-settings/usage-limits.md\ndescription: Authentication methods for Chat Thing MCP\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Add it to your client''s MCP config as a bearer token in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key on the Connect agent page and copy it.\n- type: oauth2\n  name: Browser approval\n  evidence: Your assistant opens a Chat Thing page, you click **Approve**, and it's issued a token automatically.\n  how_to_obtain: Approve the assistant in the browser when it opens the Authorize page.\ndocs: https://chatthing.ai/docs/mcp/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/chatthing-ai/authentication/chatthing-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI Chatbot
- Customer Service
- Lead Capture
- Appointment Booking
- Voice Assistant
- Internal knowledge base
- SDK
---
