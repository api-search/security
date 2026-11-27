---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: kelam-sh-allowlist-number-api-openapi.yml
  format: yaml
  label: Nousdata Inc. Allowlist Number API
  slug: kelam-sh-allowlist-number-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kelam-sh/openapi/kelam-sh-allowlist-number-api-openapi.yml
- filename: kelam-sh-balance-api-openapi.yml
  format: yaml
  label: Nousdata Inc. Balance API
  slug: kelam-sh-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kelam-sh/openapi/kelam-sh-balance-api-openapi.yml
- filename: kelam-sh-build-api-openapi.yml
  format: yaml
  label: Nousdata Inc. Build API
  slug: kelam-sh-build-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kelam-sh/openapi/kelam-sh-build-api-openapi.yml
- filename: kelam-sh-build-view-api-openapi.yml
  format: yaml
  label: Nousdata Inc. Build View API
  slug: kelam-sh-build-view-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kelam-sh/openapi/kelam-sh-build-view-api-openapi.yml
- filename: kelam-sh-call-status-api-openapi.yml
  format: yaml
  label: Nousdata Inc. Call Status API
  slug: kelam-sh-call-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kelam-sh/openapi/kelam-sh-call-status-api-openapi.yml
- filename: kelam-sh-create-agent-api-openapi.yml
  format: yaml
  label: Nousdata Inc. Create Agent API
  slug: kelam-sh-create-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kelam-sh/openapi/kelam-sh-create-agent-api-openapi.yml
- filename: kelam-sh-health-api-openapi.yml
  format: yaml
  label: Nousdata Inc. Health API
  slug: kelam-sh-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kelam-sh/openapi/kelam-sh-health-api-openapi.yml
- filename: kelam-sh-list-agents-api-openapi.yml
  format: yaml
  label: Nousdata Inc. List Agents API
  slug: kelam-sh-list-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kelam-sh/openapi/kelam-sh-list-agents-api-openapi.yml
- filename: kelam-sh-place-call-api-openapi.yml
  format: yaml
  label: Nousdata Inc. Place Call API
  slug: kelam-sh-place-call-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kelam-sh/openapi/kelam-sh-place-call-api-openapi.yml
- filename: kelam-sh-top-up-api-openapi.yml
  format: yaml
  label: Nousdata Inc. Top Up API
  slug: kelam-sh-top-up-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kelam-sh/openapi/kelam-sh-top-up-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Nousdata Inc. Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nousdata Inc. secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nousdata Inc.
provider_slug: kelam-sh
scheme_count: 1
schemes:
- in: header
  name: siwx
  parameter: SIGN-IN-WITH-X
  sources:
  - openapi/kelam-sh-openapi.json
  type: apiKey
slug: kelam-sh-authentication
source_filename: kelam-sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/kelam-sh-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: siwx\n  type: apiKey\n  in: header\n  parameter: SIGN-IN-WITH-X\n  sources:\n  - openapi/kelam-sh-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/kelam-sh/authentication/kelam-sh-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- CLI
- Voice Agents
- Installer
- Homebrew
- Python
---
