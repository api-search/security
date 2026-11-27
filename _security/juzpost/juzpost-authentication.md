---
anonymous_access: false
api_key_in: []
api_specs:
- filename: juzpost-accounts-api-openapi.yml
  format: yaml
  label: JuzPost Accounts API
  slug: juzpost-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juzpost/openapi/juzpost-accounts-api-openapi.yml
- filename: juzpost-identity-api-openapi.yml
  format: yaml
  label: JuzPost Identity API
  slug: juzpost-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juzpost/openapi/juzpost-identity-api-openapi.yml
- filename: juzpost-posts-api-openapi.yml
  format: yaml
  label: JuzPost Posts API
  slug: juzpost-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juzpost/openapi/juzpost-posts-api-openapi.yml
- filename: juzpost-scheduling-api-openapi.yml
  format: yaml
  label: JuzPost Scheduling API
  slug: juzpost-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juzpost/openapi/juzpost-scheduling-api-openapi.yml
- filename: juzpost-storage-api-openapi.yml
  format: yaml
  label: JuzPost Storage API
  slug: juzpost-storage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/juzpost/openapi/juzpost-storage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: JuzPost Authentication
name_suffix: Authentication
oauth_flows: []
overview: JuzPost secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JuzPost
provider_slug: juzpost
scheme_count: 1
schemes:
- description: 'An API key created in the dashboard under Settings, General, API keys, sent as

    `Authorization: Bearer jp_live_...`. Required on every operation without exception.

    Missing, malformed, revoked or unknown tokens all produce `401` with code

    `unauthorized`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/juzpost-openapi.json
  type: http
slug: juzpost-authentication
source_filename: juzpost-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/juzpost-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    An API key created in the dashboard under Settings, General, API keys, sent as\n    `Authorization: Bearer jp_live_...`. Required on every operation without exception.\n    Missing, malformed, revoked or unknown tokens all produce `401` with code\n    `unauthorized`.\n  sources:\n  - openapi/juzpost-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/juzpost/authentication/juzpost-authentication.yml
summary_line: http · 1 scheme
tags:
- Social Media
- Scheduling
- Automation
- Artificial Intelligence
- Marketing
---
