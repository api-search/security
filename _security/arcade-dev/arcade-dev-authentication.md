---
api_key_in:
- header
api_specs:
- filename: arcade-tools-api-openapi.yml
  format: yaml
  label: Arcade Tools API
  slug: arcade-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-tools-api-openapi.yml
- filename: arcade-auth-api-openapi.yml
  format: yaml
  label: Arcade Authorization API
  slug: arcade-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-auth-api-openapi.yml
- filename: arcade-llm-api-openapi.yml
  format: yaml
  label: Arcade LLM API
  slug: arcade-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-llm-api-openapi.yml
- filename: arcade-workers-api-openapi.yml
  format: yaml
  label: Arcade Workers API
  slug: arcade-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-workers-api-openapi.yml
- filename: arcade-gateways-api-openapi.yml
  format: yaml
  label: Arcade Gateways API
  slug: arcade-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-gateways-api-openapi.yml
- filename: arcade-hooks-api-openapi.yml
  format: yaml
  label: Arcade Hooks API
  slug: arcade-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-hooks-api-openapi.yml
- filename: arcade-admin-api-openapi.yml
  format: yaml
  label: Arcade Admin API
  slug: arcade-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-admin-api-openapi.yml
- filename: arcade-plugins-api-openapi.yml
  format: yaml
  label: Arcade Plugins API
  slug: arcade-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-plugins-api-openapi.yml
- filename: arcade-operations-api-openapi.yml
  format: yaml
  label: Arcade Operations API
  slug: arcade-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-operations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Arcade Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: arcade-dev secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: arcade-dev
provider_slug: arcade-dev
scheme_count: 1
schemes:
- description: 'Enter your API key or API token in the format: Bearer <token>'
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/arcade-admin-api-openapi.yml
  - openapi/arcade-auth-api-openapi.yml
  - openapi/arcade-gateways-api-openapi.yml
  - openapi/arcade-hooks-api-openapi.yml
  - openapi/arcade-llm-api-openapi.yml
  - openapi/arcade-operations-api-openapi.yml
  - openapi/arcade-plugins-api-openapi.yml
  - openapi/arcade-tools-api-openapi.yml
  - openapi/arcade-workers-api-openapi.yml
  type: apiKey
slug: arcade-dev-authentication
source_filename: arcade-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/arcade-admin-api-openapi.yml, openapi/arcade-auth-api-openapi.yml, openapi/arcade-gateways-api-openapi.yml,\n  openapi/arcade-hooks-api-openapi.yml, openapi/arcade-llm-api-openapi.yml, openapi/arcade-operations-api-openapi.yml,\n  openapi/arcade-plugins-api-openapi.yml, openapi/arcade-tools-api-openapi.yml, openapi/arcade-workers-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Enter your API key or API token in the format: Bearer <token>'\n  sources:\n  - openapi/arcade-admin-api-openapi.yml\n  - openapi/arcade-auth-api-openapi.yml\n  - openapi/arcade-gateways-api-openapi.yml\n  - openapi/arcade-hooks-api-openapi.yml\n  - openapi/arcade-llm-api-openapi.yml\n  - openapi/arcade-operations-api-openapi.yml\n  - openapi/arcade-plugins-api-openapi.yml\n  - openapi/arcade-tools-api-openapi.yml\n  -\
  \ openapi/arcade-workers-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/authentication/arcade-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags: []
---
