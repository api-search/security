---
api_key_in: []
api_specs:
- filename: h-company-agents-api-openapi.yml
  format: yaml
  label: H Company Agents API
  slug: h-company-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-agents-api-openapi.yml
- filename: h-company-browser-profiles-api-openapi.yml
  format: yaml
  label: H Company Browser Profiles API
  slug: h-company-browser-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-browser-profiles-api-openapi.yml
- filename: h-company-environments-api-openapi.yml
  format: yaml
  label: H Company Environments API
  slug: h-company-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-environments-api-openapi.yml
- filename: h-company-quota-api-openapi.yml
  format: yaml
  label: H Company quota API
  slug: h-company-quota-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-quota-api-openapi.yml
- filename: h-company-schedules-api-openapi.yml
  format: yaml
  label: H Company Schedules API
  slug: h-company-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-schedules-api-openapi.yml
- filename: h-company-sessions-api-openapi.yml
  format: yaml
  label: H Company Sessions API
  slug: h-company-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-sessions-api-openapi.yml
- filename: h-company-skills-api-openapi.yml
  format: yaml
  label: H Company Skills API
  slug: h-company-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-skills-api-openapi.yml
- filename: h-company-vaults-api-openapi.yml
  format: yaml
  label: H Company Vaults API
  slug: h-company-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-vaults-api-openapi.yml
- filename: h-company-webhooks-api-openapi.yml
  format: yaml
  label: H Company Webhooks API
  slug: h-company-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/openapi/h-company-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: H Company Authentication
name_suffix: Authentication
oauth_flows: []
overview: H Company secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: H Company
provider_slug: h-company
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/h-company-computer-use-agents-openapi-original.json
  type: http
slug: h-company-authentication
source_filename: h-company-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/h-company-computer-use-agents-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/h-company-computer-use-agents-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/h-company/refs/heads/main/authentication/h-company-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Agents
- Computer Use
- Automation
- Machine Learning
- Browser Automation
- LLMs
- MCP
- Developer Tools
---
