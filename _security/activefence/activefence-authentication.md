---
api_key_in:
- header
api_specs:
- filename: activefence-api-keys-api-openapi.yml
  format: yaml
  label: ActiveFence api keys API
  slug: activefence-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-api-keys-api-openapi.yml
- filename: activefence-collection-api-openapi.yml
  format: yaml
  label: ActiveFence Collection API
  slug: activefence-collection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-collection-api-openapi.yml
- filename: activefence-content-api-openapi.yml
  format: yaml
  label: ActiveFence Content API
  slug: activefence-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-content-api-openapi.yml
- filename: activefence-flags-api-openapi.yml
  format: yaml
  label: ActiveFence Flags API
  slug: activefence-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-flags-api-openapi.yml
- filename: activefence-users-api-openapi.yml
  format: yaml
  label: ActiveFence Users API
  slug: activefence-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-users-api-openapi.yml
- filename: activefence-wonderbuild-api-openapi.yml
  format: yaml
  label: ActiveFence Wonder Build API
  slug: activefence-wonderbuild-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-wonderbuild-api-openapi.yml
- filename: activefence-wonderfence-api-openapi.yml
  format: yaml
  label: ActiveFence Wonder Fence API
  slug: activefence-wonderfence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/openapi/activefence-wonderfence-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Activefence Authentication
name_suffix: Authentication
oauth_flows: []
overview: ActiveFence secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ActiveFence
provider_slug: activefence
scheme_count: 1
schemes:
- description: ''
  in: header
  name: API Key
  parameter: af-api-key
  sources:
  - openapi/activefence-alice-api-openapi.yml
  type: apiKey
slug: activefence-authentication
source_filename: activefence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: derived\nsource: openapi/activefence-alice-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: API Key\n  type: apiKey\n  in: header\n  parameter: af-api-key\n  description: ''\n  sources:\n  - openapi/activefence-alice-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/activefence/refs/heads/main/authentication/activefence-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- AI Safety
- AI Security
- Trust and Safety
- Content Moderation
- Guardrails
- Red Teaming
- LLM Security
- Prompt Injection
- AI Governance
- Risk Scoring
- User Generated Content
- Child Safety
---
