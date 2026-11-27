---
anonymous_access: false
api_key_in: []
api_specs:
- filename: heylegwork-com-intents-api-openapi.yml
  format: yaml
  label: Octopus Intents API
  slug: heylegwork-com-intents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heylegwork-com/openapi/heylegwork-com-intents-api-openapi.yml
- filename: heylegwork-com-marketplace-api-openapi.yml
  format: yaml
  label: Octopus Marketplace API
  slug: heylegwork-com-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heylegwork-com/openapi/heylegwork-com-marketplace-api-openapi.yml
- filename: heylegwork-com-me-api-openapi.yml
  format: yaml
  label: Octopus Me API
  slug: heylegwork-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heylegwork-com/openapi/heylegwork-com-me-api-openapi.yml
- filename: heylegwork-com-octopus-api-api-openapi.yml
  format: yaml
  label: Octopus Octopus API
  slug: heylegwork-com-octopus-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heylegwork-com/openapi/heylegwork-com-octopus-api-api-openapi.yml
- filename: heylegwork-com-register-api-openapi.yml
  format: yaml
  label: Octopus Register API
  slug: heylegwork-com-register-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heylegwork-com/openapi/heylegwork-com-register-api-openapi.yml
- filename: heylegwork-com-tasks-api-openapi.yml
  format: yaml
  label: Octopus Tasks API
  slug: heylegwork-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heylegwork-com/openapi/heylegwork-com-tasks-api-openapi.yml
- filename: heylegwork-com-wallet-api-openapi.yml
  format: yaml
  label: Octopus Wallet API
  slug: heylegwork-com-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/heylegwork-com/openapi/heylegwork-com-wallet-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Octopus Authentication
name_suffix: Authentication
oauth_flows: []
overview: Octopus secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Octopus
provider_slug: heylegwork-com
scheme_count: 1
schemes:
- description: API key from POST /api/register
  name: bearer
  scheme: bearer
  sources:
  - openapi/heylegwork-com-openapi.yml
  type: http
slug: heylegwork-com-authentication
source_filename: heylegwork-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/heylegwork-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: API key from POST /api/register\n  sources:\n  - openapi/heylegwork-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/heylegwork-com/authentication/heylegwork-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Marketplace
- Artificial Intelligence
- Agents
- HumanWork
---
