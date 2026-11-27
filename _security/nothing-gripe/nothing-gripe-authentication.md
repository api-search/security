---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nothing-gripe-agent-api-openapi.yml
  format: yaml
  label: Nothing.gripe Agent API
  slug: nothing-gripe-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothing-gripe/openapi/nothing-gripe-agent-api-openapi.yml
- filename: nothing-gripe-doer-api-openapi.yml
  format: yaml
  label: Nothing.gripe Doer API
  slug: nothing-gripe-doer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothing-gripe/openapi/nothing-gripe-doer-api-openapi.yml
- filename: nothing-gripe-tasks-api-openapi.yml
  format: yaml
  label: Nothing.gripe Tasks API
  slug: nothing-gripe-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nothing-gripe/openapi/nothing-gripe-tasks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Nothing.gripe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nothing.gripe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nothing.gripe
provider_slug: nothing-gripe
scheme_count: 1
schemes:
- description: '"Doer <session token>" from /api/doer/finish, or "Doer ak_..." agent key from /api/agent/key.'
  in: header
  name: doerAuth
  parameter: Authorization
  sources:
  - openapi/nothing-gripe-openapi.json
  type: apiKey
slug: nothing-gripe-authentication
source_filename: nothing-gripe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nothing-gripe-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: doerAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: '\"Doer <session token>\" from /api/doer/finish, or \"Doer ak_...\" agent key from\n    /api/agent/key.'\n  sources:\n  - openapi/nothing-gripe-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nothing-gripe/authentication/nothing-gripe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Marketplace
- Task
- Cryptocurrency
- Funding
- Platform
- Company
---
