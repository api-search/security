---
api_key_in: []
api_specs:
- filename: activepieces.json
  format: json
  label: Activepieces API
  slug: activepieces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/openapi/activepieces.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Activepieces Authentication
name_suffix: Authentication
oauth_flows: []
overview: Activepieces secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Activepieces
provider_slug: activepieces
scheme_count: 1
schemes:
- description: API key from the Activepieces admin console, passed as a Bearer token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/activepieces.json
  type: http
slug: activepieces-authentication
source_filename: activepieces-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/activepieces.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key from the Activepieces admin console, passed as a Bearer token\n  sources:\n  - openapi/activepieces.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activepieces/refs/heads/main/authentication/activepieces-authentication.yml
summary_line: http · 1 scheme
tags:
- Automation
- No-Code
- Open Source
- Workflow
- AI Agents
- MCP
---
