---
api_key_in:
- header
api_specs:
- filename: arcade-dev-admin-api-openapi.yml
  format: yaml
  label: arcade-dev Admin API
  slug: arcade-dev-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-admin-api-openapi.yml
- filename: arcade-dev-authorization-api-openapi.yml
  format: yaml
  label: arcade-dev Authorization API
  slug: arcade-dev-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-authorization-api-openapi.yml
- filename: arcade-dev-gateways-api-openapi.yml
  format: yaml
  label: arcade-dev Gateways API
  slug: arcade-dev-gateways-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-gateways-api-openapi.yml
- filename: arcade-dev-hooks-api-openapi.yml
  format: yaml
  label: arcade-dev Hooks API
  slug: arcade-dev-hooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-hooks-api-openapi.yml
- filename: arcade-dev-llm-api-openapi.yml
  format: yaml
  label: arcade-dev LLM API
  slug: arcade-dev-llm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-llm-api-openapi.yml
- filename: arcade-dev-operations-api-openapi.yml
  format: yaml
  label: arcade-dev Operations API
  slug: arcade-dev-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-operations-api-openapi.yml
- filename: arcade-dev-plugins-api-openapi.yml
  format: yaml
  label: arcade-dev Plugins API
  slug: arcade-dev-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-plugins-api-openapi.yml
- filename: arcade-dev-tools-api-openapi.yml
  format: yaml
  label: arcade-dev Tools API
  slug: arcade-dev-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/arcade-dev/refs/heads/main/openapi/arcade-dev-tools-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Arcade Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arcade.dev secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Arcade.dev
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
