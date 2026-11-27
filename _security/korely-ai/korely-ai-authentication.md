---
anonymous_access: false
api_key_in: []
api_specs:
- filename: korely-ai-account-api-openapi.yml
  format: yaml
  label: Korely Account API
  slug: korely-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-account-api-openapi.yml
- filename: korely-ai-admin-api-openapi.yml
  format: yaml
  label: Korely Admin API
  slug: korely-ai-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-admin-api-openapi.yml
- filename: korely-ai-agents-api-openapi.yml
  format: yaml
  label: Korely Agents API
  slug: korely-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-agents-api-openapi.yml
- filename: korely-ai-audit-api-openapi.yml
  format: yaml
  label: Korely Audit API
  slug: korely-ai-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-audit-api-openapi.yml
- filename: korely-ai-batch-api-openapi.yml
  format: yaml
  label: Korely Batch API
  slug: korely-ai-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-batch-api-openapi.yml
- filename: korely-ai-context-api-openapi.yml
  format: yaml
  label: Korely Context API
  slug: korely-ai-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-context-api-openapi.yml
- filename: korely-ai-events-api-openapi.yml
  format: yaml
  label: Korely Events API
  slug: korely-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-events-api-openapi.yml
- filename: korely-ai-facts-api-openapi.yml
  format: yaml
  label: Korely Facts API
  slug: korely-ai-facts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-facts-api-openapi.yml
- filename: korely-ai-hosted-api-openapi.yml
  format: yaml
  label: Korely Hosted API
  slug: korely-ai-hosted-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-hosted-api-openapi.yml
- filename: korely-ai-memories-api-openapi.yml
  format: yaml
  label: Korely Memories API
  slug: korely-ai-memories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-memories-api-openapi.yml
- filename: korely-ai-oauth-api-openapi.yml
  format: yaml
  label: Korely OAuth API
  slug: korely-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-oauth-api-openapi.yml
- filename: korely-ai-ops-api-openapi.yml
  format: yaml
  label: Korely Ops API
  slug: korely-ai-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-ops-api-openapi.yml
- filename: korely-ai-ping-api-openapi.yml
  format: yaml
  label: Korely Ping API
  slug: korely-ai-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-ping-api-openapi.yml
- filename: korely-ai-profile-api-openapi.yml
  format: yaml
  label: Korely Profile API
  slug: korely-ai-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-profile-api-openapi.yml
- filename: korely-ai-users-api-openapi.yml
  format: yaml
  label: Korely Users API
  slug: korely-ai-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korely-ai/openapi/korely-ai-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Korely Authentication
name_suffix: Authentication
oauth_flows: []
overview: Korely secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Korely
provider_slug: korely-ai
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/korely-ai-agent-openapi.json
  - openapi/korely-ai-openapi.json
  type: http
slug: korely-ai-authentication
source_filename: korely-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: derived\nsource: openapi/korely-ai-agent-openapi.json, openapi/korely-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/korely-ai-agent-openapi.json\n  - openapi/korely-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/korely-ai/authentication/korely-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Memory
- Bi-temporal
- Agents
---
