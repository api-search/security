---
anonymous_access: false
api_key_in: []
api_specs:
- filename: modly-cc-guild-api-openapi.yml
  format: yaml
  label: Modly Guild API
  slug: modly-cc-guild-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modly-cc/openapi/modly-cc-guild-api-openapi.yml
- filename: modly-cc-leveling-api-openapi.yml
  format: yaml
  label: Modly Leveling API
  slug: modly-cc-leveling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modly-cc/openapi/modly-cc-leveling-api-openapi.yml
- filename: modly-cc-moderation-api-openapi.yml
  format: yaml
  label: Modly Moderation API
  slug: modly-cc-moderation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modly-cc/openapi/modly-cc-moderation-api-openapi.yml
- filename: modly-cc-modules-api-openapi.yml
  format: yaml
  label: Modly Modules API
  slug: modly-cc-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modly-cc/openapi/modly-cc-modules-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Modly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Modly
provider_slug: modly-cc
scheme_count: 1
schemes:
- description: 'Authorization: Bearer mdly_…'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/modly-cc-openapi.json
  type: http
slug: modly-cc-authentication
source_filename: modly-cc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/modly-cc-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer mdly_…'\n  sources:\n  - openapi/modly-cc-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/modly-cc/authentication/modly-cc-authentication.yml
summary_line: http · 1 scheme
tags:
- Discord
- Bot
- Moderation
- Artificial Intelligence
- Community
---
