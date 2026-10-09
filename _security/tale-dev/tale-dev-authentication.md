---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tale-dev-agents-api-openapi.yml
  format: yaml
  label: Tale Agents API
  slug: tale-dev-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-agents-api-openapi.yml
- filename: tale-dev-automations-api-openapi.yml
  format: yaml
  label: Tale Automations API
  slug: tale-dev-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-automations-api-openapi.yml
- filename: tale-dev-browser-sessions-api-openapi.yml
  format: yaml
  label: Tale Browser sessions API
  slug: tale-dev-browser-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-browser-sessions-api-openapi.yml
- filename: tale-dev-contacts-api-openapi.yml
  format: yaml
  label: Tale Contacts API
  slug: tale-dev-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-contacts-api-openapi.yml
- filename: tale-dev-conversations-api-openapi.yml
  format: yaml
  label: Tale Conversations API
  slug: tale-dev-conversations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-conversations-api-openapi.yml
- filename: tale-dev-documents-api-openapi.yml
  format: yaml
  label: Tale Documents API
  slug: tale-dev-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-documents-api-openapi.yml
- filename: tale-dev-knowledge-api-openapi.yml
  format: yaml
  label: Tale Knowledge API
  slug: tale-dev-knowledge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-knowledge-api-openapi.yml
- filename: tale-dev-mcp-api-openapi.yml
  format: yaml
  label: Tale MCP API
  slug: tale-dev-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-mcp-api-openapi.yml
- filename: tale-dev-model-endpoints-api-openapi.yml
  format: yaml
  label: Tale Model endpoints API
  slug: tale-dev-model-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-model-endpoints-api-openapi.yml
- filename: tale-dev-notifications-api-openapi.yml
  format: yaml
  label: Tale Notifications API
  slug: tale-dev-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-notifications-api-openapi.yml
- filename: tale-dev-organization-api-openapi.yml
  format: yaml
  label: Tale Organization API
  slug: tale-dev-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-organization-api-openapi.yml
- filename: tale-dev-products-api-openapi.yml
  format: yaml
  label: Tale Products API
  slug: tale-dev-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-products-api-openapi.yml
- filename: tale-dev-projects-api-openapi.yml
  format: yaml
  label: Tale Projects API
  slug: tale-dev-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-projects-api-openapi.yml
- filename: tale-dev-runs-api-openapi.yml
  format: yaml
  label: Tale Runs API
  slug: tale-dev-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-runs-api-openapi.yml
- filename: tale-dev-skills-api-openapi.yml
  format: yaml
  label: Tale Skills API
  slug: tale-dev-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-skills-api-openapi.yml
- filename: tale-dev-tasks-api-openapi.yml
  format: yaml
  label: Tale Tasks API
  slug: tale-dev-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-tasks-api-openapi.yml
- filename: tale-dev-threads-api-openapi.yml
  format: yaml
  label: Tale Threads API
  slug: tale-dev-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-threads-api-openapi.yml
- filename: tale-dev-websites-api-openapi.yml
  format: yaml
  label: Tale Websites API
  slug: tale-dev-websites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/openapi/tale-dev-websites-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Tale Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tale secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tale
provider_slug: tale-dev
scheme_count: 1
schemes:
- description: An organization API key. Create one in Settings → API. Pasted into the explorer on /docs it stays in the page’s memory only and is forgotten on reload — it is never stored.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/tale-dev-openapi.yml
  type: http
slug: tale-dev-authentication
source_filename: tale-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: derived\nsource: openapi/tale-dev-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: An organization API key. Create one in Settings → API. Pasted into the explorer\n    on /docs it stays in the page’s memory only and is forgotten on reload — it is never stored.\n  sources:\n  - openapi/tale-dev-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tale-dev/refs/heads/main/authentication/tale-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Agents
- Automation
- Knowledge Management
- MCP
- Open Source
- Self-Hosted
---
