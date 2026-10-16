---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hourtick-v1-openapi.json
  format: json
  label: Hourtick API V1 API
  slug: hourtick-api-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/_original/hourtick-v1-openapi.json
auth_types: []
description: Authentication methods published by Hourtick
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hourtick Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hourtick declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hourtick
provider_slug: hourtick
scheme_count: 2
schemes:
- evidence: Create a token Settings → API tokens → Create. Copy it once; we only store a hash.
  header: Authorization
  how_to_obtain: Create a personal token in Settings → API tokens → Create.
  location: header
  name: Personal token
  type: http-bearer
- evidence: Hourtick's MCP server now supports OAuth 2.1, so Claude.ai, Claude Desktop, ChatGPT and other apps connect by signing in to Hourtick instead of pasting a token.
  how_to_obtain: Sign in on hourtick.com and approve the connection.
  name: OAuth 2.1 sign‑in
  type: oauth2
slug: hourtick-authentication
source_filename: hourtick-authentication.yml
source_heading: Authentication Profile
source_url: https://hourtick.com/guides/true-cost-of-ai-agent-work
source_yaml: "generated: '2026-10-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hourtick.com/guides/true-cost-of-ai-agent-work\nsources:\n- https://hourtick.com/guides/true-cost-of-ai-agent-work\n- https://hourtick.com/announcements/connect-chatgpt-and-claude\n- https://hourtick.com/developers\ndescription: Authentication methods published by Hourtick\nschemes:\n- type: http-bearer\n  name: Personal token\n  evidence: Create a token Settings → API tokens → Create. Copy it once; we only store a hash.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a personal token in Settings → API tokens → Create.\n- type: oauth2\n  name: OAuth 2.1 sign‑in\n  evidence: Hourtick's MCP server now supports OAuth 2.1, so Claude.ai, Claude Desktop, ChatGPT and other apps connect by signing in to Hourtick\n    instead of pasting a token.\n  how_to_obtain: Sign in on hourtick.com and approve the connection.\ndocs: https://hourtick.com/guides/true-cost-of-ai-agent-work\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/authentication/hourtick-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Collaboration
- AI
- TimeTracking
- ProjectManagement
---
