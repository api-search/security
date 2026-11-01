---
anonymous_access: false
api_key_in:
- cookie
api_specs:
- filename: giljo-ai-account-deletion-api-openapi.yml
  format: yaml
  label: giljo-ai Account Deletion API
  slug: giljo-ai-account-deletion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-account-deletion-api-openapi.yml
- filename: giljo-ai-account-lifecycle-api-openapi.yml
  format: yaml
  label: giljo-ai Account Lifecycle API
  slug: giljo-ai-account-lifecycle-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-account-lifecycle-api-openapi.yml
- filename: giljo-ai-auth-api-openapi.yml
  format: yaml
  label: giljo-ai Auth API
  slug: giljo-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-auth-api-openapi.yml
- filename: giljo-ai-comm-threads-api-openapi.yml
  format: yaml
  label: giljo-ai Comm Threads API
  slug: giljo-ai-comm-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-comm-threads-api-openapi.yml
- filename: giljo-ai-connected-accounts-api-openapi.yml
  format: yaml
  label: giljo-ai Connected Accounts API
  slug: giljo-ai-connected-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-connected-accounts-api-openapi.yml
- filename: giljo-ai-health-api-openapi.yml
  format: yaml
  label: giljo-ai Health API
  slug: giljo-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-health-api-openapi.yml
- filename: giljo-ai-legal-api-openapi.yml
  format: yaml
  label: giljo-ai Legal API
  slug: giljo-ai-legal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-legal-api-openapi.yml
- filename: giljo-ai-oauth-api-openapi.yml
  format: yaml
  label: giljo-ai OAuth API
  slug: giljo-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-oauth-api-openapi.yml
- filename: giljo-ai-oauth-dcr-api-openapi.yml
  format: yaml
  label: giljo-ai OAUTH Dcr API
  slug: giljo-ai-oauth-dcr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-oauth-dcr-api-openapi.yml
- filename: giljo-ai-social-login-api-openapi.yml
  format: yaml
  label: giljo-ai Social Login API
  slug: giljo-ai-social-login-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-social-login-api-openapi.yml
- filename: giljo-ai-task-statuses-api-openapi.yml
  format: yaml
  label: giljo-ai Task Statuses API
  slug: giljo-ai-task-statuses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-task-statuses-api-openapi.yml
- filename: giljo-ai-tasks-api-openapi.yml
  format: yaml
  label: giljo-ai Tasks API
  slug: giljo-ai-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-tasks-api-openapi.yml
- filename: giljo-ai-users-api-openapi.yml
  format: yaml
  label: giljo-ai Users API
  slug: giljo-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/giljo-ai/openapi/giljo-ai-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Giljo Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: giljo-ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: giljo-ai
provider_slug: giljo-ai
scheme_count: 1
schemes:
- in: cookie
  name: CookieSession
  parameter: access_token
  sources:
  - openapi/amh-openapi.json
  type: apiKey
slug: giljo-ai-authentication
source_filename: giljo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/amh-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: CookieSession\n  type: apiKey\n  in: cookie\n  parameter: access_token\n  sources:\n  - openapi/amh-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/giljo-ai/authentication/giljo-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- AI
- Agent
- Collaboration
- Platform
---
