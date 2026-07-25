---
api_key_in:
- header
api_specs:
- filename: alice-api-keys-api-openapi.yml
  format: yaml
  label: Alice api keys API
  slug: alice-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-api-keys-api-openapi.yml
- filename: alice-collection-api-openapi.yml
  format: yaml
  label: Alice collection API
  slug: alice-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-collection-api-openapi.yml
- filename: alice-content-api-openapi.yml
  format: yaml
  label: Alice content API
  slug: alice-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-content-api-openapi.yml
- filename: alice-flags-api-openapi.yml
  format: yaml
  label: Alice flags API
  slug: alice-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-flags-api-openapi.yml
- filename: alice-users-api-openapi.yml
  format: yaml
  label: Alice users API
  slug: alice-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-users-api-openapi.yml
- filename: alice-wonderbuild-api-openapi.yml
  format: yaml
  label: Alice WonderBuild API
  slug: alice-wonderbuild-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-wonderbuild-api-openapi.yml
- filename: alice-wonderfence-api-openapi.yml
  format: yaml
  label: Alice WonderFence API
  slug: alice-wonderfence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/openapi/alice-wonderfence-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Alice Authentication
name_suffix: Authentication
oauth_flows: []
overview: Alice secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Alice
provider_slug: alice
scheme_count: 1
schemes:
- description: ''
  in: header
  name: API Key
  parameter: af-api-key
  sources:
  - openapi/alice-openapi-original.json
  type: apiKey
slug: alice-authentication
source_filename: alice-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: derived\nsource: openapi/alice-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: af-api-key\n  description: ''\n  sources:\n  - openapi/alice-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alice/refs/heads/main/authentication/alice-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Developer Tools
- AI Security
- AI Safety
- Content Moderation
- Trust and Safety
- LLM Guardrails
- Red Teaming
- GenAI
---
