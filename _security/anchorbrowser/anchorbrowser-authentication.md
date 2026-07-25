---
api_key_in:
- header
api_specs:
- filename: anchorbrowser-agentic-capabilities-api-openapi.yml
  format: yaml
  label: Anchor Browser Agentic capabilities API
  slug: anchorbrowser-agentic-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-agentic-capabilities-api-openapi.yml
- filename: anchorbrowser-ai-tools-api-openapi.yml
  format: yaml
  label: Anchor Browser AI Tools API
  slug: anchorbrowser-ai-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-ai-tools-api-openapi.yml
- filename: anchorbrowser-applications-api-openapi.yml
  format: yaml
  label: Anchor Browser Applications API
  slug: anchorbrowser-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-applications-api-openapi.yml
- filename: anchorbrowser-batch-sessions-api-openapi.yml
  format: yaml
  label: Anchor Browser Batch Sessions API
  slug: anchorbrowser-batch-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-batch-sessions-api-openapi.yml
- filename: anchorbrowser-billing-api-openapi.yml
  format: yaml
  label: Anchor Browser Billing API
  slug: anchorbrowser-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-billing-api-openapi.yml
- filename: anchorbrowser-browser-sessions-api-openapi.yml
  format: yaml
  label: Anchor Browser Browser Sessions API
  slug: anchorbrowser-browser-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-browser-sessions-api-openapi.yml
- filename: anchorbrowser-certificates-api-openapi.yml
  format: yaml
  label: Anchor Browser Certificates API
  slug: anchorbrowser-certificates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-certificates-api-openapi.yml
- filename: anchorbrowser-event-coordination-api-openapi.yml
  format: yaml
  label: Anchor Browser Event Coordination API
  slug: anchorbrowser-event-coordination-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-event-coordination-api-openapi.yml
- filename: anchorbrowser-extensions-api-openapi.yml
  format: yaml
  label: Anchor Browser Extensions API
  slug: anchorbrowser-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-extensions-api-openapi.yml
- filename: anchorbrowser-identities-api-openapi.yml
  format: yaml
  label: Anchor Browser Identities API
  slug: anchorbrowser-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-identities-api-openapi.yml
- filename: anchorbrowser-integrations-api-openapi.yml
  format: yaml
  label: Anchor Browser Integrations API
  slug: anchorbrowser-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-integrations-api-openapi.yml
- filename: anchorbrowser-os-level-control-api-openapi.yml
  format: yaml
  label: Anchor Browser OS Level Control API
  slug: anchorbrowser-os-level-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-os-level-control-api-openapi.yml
- filename: anchorbrowser-profiles-api-openapi.yml
  format: yaml
  label: Anchor Browser Profiles API
  slug: anchorbrowser-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-profiles-api-openapi.yml
- filename: anchorbrowser-session-recordings-api-openapi.yml
  format: yaml
  label: Anchor Browser Session Recordings API
  slug: anchorbrowser-session-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-session-recordings-api-openapi.yml
- filename: anchorbrowser-tasks-api-openapi.yml
  format: yaml
  label: Anchor Browser Tasks API
  slug: anchorbrowser-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-tasks-api-openapi.yml
- filename: anchorbrowser-tasks-legacy-api-openapi.yml
  format: yaml
  label: Anchor Browser Tasks (Legacy) API
  slug: anchorbrowser-tasks-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-tasks-legacy-api-openapi.yml
- filename: anchorbrowser-tools-api-openapi.yml
  format: yaml
  label: Anchor Browser Tools API
  slug: anchorbrowser-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/openapi/anchorbrowser-tools-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Anchorbrowser Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anchor Browser secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Anchor Browser
provider_slug: anchorbrowser
scheme_count: 1
schemes:
- description: API key passed in the header
  in: header
  name: api_key_header
  parameter: anchor-api-key
  sources:
  - openapi/anchorbrowser-openapi.yml
  type: apiKey
slug: anchorbrowser-authentication
source_filename: anchorbrowser-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/anchorbrowser-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key_header\n  type: apiKey\n  in: header\n  parameter: anchor-api-key\n  description: API key passed in the header\n  sources:\n  - openapi/anchorbrowser-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anchorbrowser/refs/heads/main/authentication/anchorbrowser-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Browser Infrastructure
- AI Agents
- Cloud Browser
- Browser Automation
- Sandbox
- Stealth Browser
- MCP
---
