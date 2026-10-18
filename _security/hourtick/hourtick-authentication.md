---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hourtick-account-api-openapi.yml
  format: yaml
  label: Hourtick Account API
  slug: hourtick-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-account-api-openapi.yml
- filename: hourtick-agents-api-openapi.yml
  format: yaml
  label: Hourtick Agents API
  slug: hourtick-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-agents-api-openapi.yml
- filename: hourtick-billing-api-openapi.yml
  format: yaml
  label: Hourtick Billing API
  slug: hourtick-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-billing-api-openapi.yml
- filename: hourtick-catalog-api-openapi.yml
  format: yaml
  label: Hourtick Catalog API
  slug: hourtick-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-catalog-api-openapi.yml
- filename: hourtick-chat-api-openapi.yml
  format: yaml
  label: Hourtick Chat API
  slug: hourtick-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-chat-api-openapi.yml
- filename: hourtick-integrations-api-openapi.yml
  format: yaml
  label: Hourtick Integrations API
  slug: hourtick-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-integrations-api-openapi.yml
- filename: hourtick-invoices-api-openapi.yml
  format: yaml
  label: Hourtick Invoices API
  slug: hourtick-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-invoices-api-openapi.yml
- filename: hourtick-notes-and-files-api-openapi.yml
  format: yaml
  label: Hourtick Notes and files API
  slug: hourtick-notes-and-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-notes-and-files-api-openapi.yml
- filename: hourtick-reports-api-openapi.yml
  format: yaml
  label: Hourtick Reports API
  slug: hourtick-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-reports-api-openapi.yml
- filename: hourtick-tasks-api-openapi.yml
  format: yaml
  label: Hourtick Tasks API
  slug: hourtick-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-tasks-api-openapi.yml
- filename: hourtick-team-api-openapi.yml
  format: yaml
  label: Hourtick Team API
  slug: hourtick-team-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-team-api-openapi.yml
- filename: hourtick-time-api-openapi.yml
  format: yaml
  label: Hourtick Time API
  slug: hourtick-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hourtick/refs/heads/main/openapi/hourtick-time-api-openapi.yml
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
- Artificial Intelligence
- TimeTracking
- Project Management
---
