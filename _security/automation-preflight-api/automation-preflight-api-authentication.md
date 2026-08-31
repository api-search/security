---
api_key_in:
- header
api_specs:
- filename: automation-preflight-api-acceptance-pack-api-openapi.yml
  format: yaml
  label: Automation Preflight API Acceptance Pack API
  slug: automation-preflight-api-acceptance-pack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-acceptance-pack-api-openapi.yml
- filename: automation-preflight-api-analyze-api-openapi.yml
  format: yaml
  label: Automation Preflight API Analyze API
  slug: automation-preflight-api-analyze-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-analyze-api-openapi.yml
- filename: automation-preflight-api-direct-api-openapi.yml
  format: yaml
  label: Automation Preflight API Direct API
  slug: automation-preflight-api-direct-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-direct-api-openapi.yml
- filename: automation-preflight-api-health-api-openapi.yml
  format: yaml
  label: Automation Preflight API Health API
  slug: automation-preflight-api-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/openapi/automation-preflight-api-health-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Automation Preflight Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Automation Preflight API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Automation Preflight API
provider_slug: automation-preflight-api
scheme_count: 1
schemes:
- description: Use the Gumroad license key shown in the purchase receipt and download page, or a key issued directly by TinyOps Studio.
  in: header
  name: TinyOpsApiKey
  parameter: X-TinyOps-API-Key
  sources:
  - openapi/automation-preflight-api-direct-openapi.json
  type: apiKey
slug: automation-preflight-api-authentication
source_filename: automation-preflight-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/automation-preflight-api-direct-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TinyOpsApiKey\n  type: apiKey\n  in: header\n  parameter: X-TinyOps-API-Key\n  description: Use the Gumroad license key shown in the purchase receipt and download page,\n    or a key issued directly by TinyOps Studio.\n  sources:\n  - openapi/automation-preflight-api-direct-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automation-preflight-api/refs/heads/main/authentication/automation-preflight-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- automation
- integration
- Developer Tools
- readiness
- Testing
- url-analysis
- Web Scraping
- agent-tools
- quality-assurance
- site-audit
---
