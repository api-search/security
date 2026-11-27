---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mutator-app-analytics-api-openapi.yml
  format: yaml
  label: Mutator Analytics API
  slug: mutator-app-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-analytics-api-openapi.yml
- filename: mutator-app-approvals-api-openapi.yml
  format: yaml
  label: Mutator Approvals API
  slug: mutator-app-approvals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-approvals-api-openapi.yml
- filename: mutator-app-assets-api-openapi.yml
  format: yaml
  label: Mutator Assets API
  slug: mutator-app-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-assets-api-openapi.yml
- filename: mutator-app-automations-api-openapi.yml
  format: yaml
  label: Mutator Automations API
  slug: mutator-app-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-automations-api-openapi.yml
- filename: mutator-app-generations-api-openapi.yml
  format: yaml
  label: Mutator Generations API
  slug: mutator-app-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-generations-api-openapi.yml
- filename: mutator-app-hooks-api-openapi.yml
  format: yaml
  label: Mutator Hooks API
  slug: mutator-app-hooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-hooks-api-openapi.yml
- filename: mutator-app-index-api-openapi.yml
  format: yaml
  label: Mutator Index API
  slug: mutator-app-index-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-index-api-openapi.yml
- filename: mutator-app-media-api-openapi.yml
  format: yaml
  label: Mutator Media API
  slug: mutator-app-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-media-api-openapi.yml
- filename: mutator-app-posts-api-openapi.yml
  format: yaml
  label: Mutator Posts API
  slug: mutator-app-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-posts-api-openapi.yml
- filename: mutator-app-runs-api-openapi.yml
  format: yaml
  label: Mutator Runs API
  slug: mutator-app-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mutator-app/openapi/mutator-app-runs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Mutator Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mutator secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mutator
provider_slug: mutator-app
scheme_count: 1
schemes:
- description: 'A Mutator API key: Settings, API keys, New key.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mutator-app-openapi.json
  type: http
slug: mutator-app-authentication
source_filename: mutator-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mutator-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'A Mutator API key: Settings, API keys, New key.'\n  sources:\n  - openapi/mutator-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mutator-app/authentication/mutator-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Video
- UGC
- Marketing
- Platform
---
