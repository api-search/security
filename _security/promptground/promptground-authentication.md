---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: promptground-api-v1-api-openapi.yml
  format: yaml
  label: PromptGround API v1 API
  slug: promptground-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-api-v1-api-openapi.yml
- filename: promptground-api-v2-api-openapi.yml
  format: yaml
  label: PromptGround API v2 API
  slug: promptground-api-v2-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-api-v2-api-openapi.yml
- filename: promptground-invites-api-openapi.yml
  format: yaml
  label: PromptGround Invites API
  slug: promptground-invites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-invites-api-openapi.yml
- filename: promptground-models-api-openapi.yml
  format: yaml
  label: PromptGround Models API
  slug: promptground-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-models-api-openapi.yml
- filename: promptground-payments-api-openapi.yml
  format: yaml
  label: PromptGround Payments API
  slug: promptground-payments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-payments-api-openapi.yml
- filename: promptground-projects-api-openapi.yml
  format: yaml
  label: PromptGround Projects API
  slug: promptground-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-projects-api-openapi.yml
- filename: promptground-prompts-api-openapi.yml
  format: yaml
  label: PromptGround Prompts API
  slug: promptground-prompts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-prompts-api-openapi.yml
- filename: promptground-sessions-api-openapi.yml
  format: yaml
  label: PromptGround Sessions API
  slug: promptground-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-sessions-api-openapi.yml
- filename: promptground-settings-api-openapi.yml
  format: yaml
  label: PromptGround Settings API
  slug: promptground-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/promptground/openapi/promptground-settings-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Promptground Authentication
name_suffix: Authentication
oauth_flows: []
overview: PromptGround secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PromptGround
provider_slug: promptground
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: Authorization
  sources:
  - openapi/promptground-openapi.json
  type: apiKey
slug: promptground-authentication
source_filename: promptground-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-18'\nmethod: derived\nsource: openapi/promptground-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/promptground-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/promptground/authentication/promptground-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Prompt Engineering
- Collaboration
- Analytics
- SDK
---
