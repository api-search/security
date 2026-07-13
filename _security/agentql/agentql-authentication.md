---
api_key_in:
- header
api_specs:
- filename: agentql-openapi.yaml
  format: yaml
  label: AgentQL Query Data API
  slug: query-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/openapi/agentql-openapi.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Agentql Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentQL secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AgentQL
provider_slug: agentql
scheme_count: 1
schemes:
- description: API key from the AgentQL Dev Portal (https://dev.agentql.com)
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/agentql-openapi.yaml
  type: apiKey
slug: agentql-authentication
source_filename: agentql-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/agentql-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key from the AgentQL Dev Portal (https://dev.agentql.com)\n  sources:\n  - openapi/agentql-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentql/refs/heads/main/authentication/agentql-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agents
- Artificial Intelligence
- Web Scraping
- Data Extraction
- Browser Automation
- REST API
---
