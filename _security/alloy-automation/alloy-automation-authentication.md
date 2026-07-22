---
api_key_in: []
api_specs:
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Users API
  slug: alloy-automation-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation User Tokens API
  slug: alloy-automation-user-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Credentials API
  slug: alloy-automation-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Integrations API
  slug: alloy-automation-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Connectivity API
  slug: alloy-automation-connectivity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Passthrough API
  slug: alloy-automation-passthrough-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Events API
  slug: alloy-automation-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Unified Commerce API
  slug: alloy-automation-unified-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Unified CRM API
  slug: alloy-automation-unified-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
- filename: alloy-automation-openapi.yml
  format: yaml
  label: Alloy Automation Unified Accounting API
  slug: alloy-automation-unified-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/openapi/alloy-automation-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Alloy Automation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alloy Automation secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alloy Automation
provider_slug: alloy-automation
scheme_count: 1
schemes:
- description: 'Bearer API key in the Authorization header, e.g. `Authorization: Bearer [example key]`. Frontend calls use a per-user JWT instead of the master key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/alloy-automation-openapi.yml
  type: http
slug: alloy-automation-authentication
source_filename: alloy-automation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/alloy-automation-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer API key in the Authorization header, e.g. `Authorization: Bearer [example key]`.\n    Frontend calls use a per-user JWT instead of the master key.'\n  sources:\n  - openapi/alloy-automation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alloy-automation/refs/heads/main/authentication/alloy-automation-authentication.yml
summary_line: http · 1 scheme
tags:
- iPaaS
- Integration
- Unified API
- Embedded
- SaaS
- Automation
---
