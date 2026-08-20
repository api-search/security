---
api_key_in:
- header
api_specs:
- filename: budibase-applications-api-openapi.yml
  format: yaml
  label: Budibase Applications API
  slug: budibase-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-applications-api-openapi.yml
- filename: budibase-queries-api-openapi.yml
  format: yaml
  label: Budibase Queries API
  slug: budibase-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-queries-api-openapi.yml
- filename: budibase-rows-api-openapi.yml
  format: yaml
  label: Budibase Rows API
  slug: budibase-rows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-rows-api-openapi.yml
- filename: budibase-tables-api-openapi.yml
  format: yaml
  label: Budibase Tables API
  slug: budibase-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-tables-api-openapi.yml
- filename: budibase-users-api-openapi.yml
  format: yaml
  label: Budibase Users API
  slug: budibase-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/openapi/budibase-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Budibase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Budibase secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Budibase
provider_slug: budibase
scheme_count: 1
schemes:
- description: API key generated from the Budibase portal user dropdown menu.
  in: header
  name: apiKeyAuth
  parameter: x-budibase-api-key
  sources:
  - openapi/budibase-openapi.yml
  type: apiKey
slug: budibase-authentication
source_filename: budibase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/budibase-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-budibase-api-key\n  description: API key generated from the Budibase portal user dropdown menu.\n  sources:\n  - openapi/budibase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/budibase/refs/heads/main/authentication/budibase-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Agents
- Automation
- Internal Tools
- Low-Code
- Open-Source
- Workflow-Automation
---
