---
anonymous_access: false
api_key_in: []
api_specs:
- filename: antwork-io-accounts-api-openapi.yml
  format: yaml
  label: Antwork Accounts API
  slug: antwork-io-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antwork-io/openapi/antwork-io-accounts-api-openapi.yml
- filename: antwork-io-analytics-api-openapi.yml
  format: yaml
  label: Antwork Analytics API
  slug: antwork-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antwork-io/openapi/antwork-io-analytics-api-openapi.yml
- filename: antwork-io-campaigns-api-openapi.yml
  format: yaml
  label: Antwork Campaigns API
  slug: antwork-io-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antwork-io/openapi/antwork-io-campaigns-api-openapi.yml
- filename: antwork-io-media-api-openapi.yml
  format: yaml
  label: Antwork Media API
  slug: antwork-io-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antwork-io/openapi/antwork-io-media-api-openapi.yml
- filename: antwork-io-platforms-api-openapi.yml
  format: yaml
  label: Antwork Platforms API
  slug: antwork-io-platforms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antwork-io/openapi/antwork-io-platforms-api-openapi.yml
- filename: antwork-io-posts-api-openapi.yml
  format: yaml
  label: Antwork Posts API
  slug: antwork-io-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antwork-io/openapi/antwork-io-posts-api-openapi.yml
- filename: antwork-io-usage-api-openapi.yml
  format: yaml
  label: Antwork Usage API
  slug: antwork-io-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antwork-io/openapi/antwork-io-usage-api-openapi.yml
- filename: antwork-io-workspaces-api-openapi.yml
  format: yaml
  label: Antwork Workspaces API
  slug: antwork-io-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/antwork-io/openapi/antwork-io-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Antwork Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Antwork secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Antwork
provider_slug: antwork-io
scheme_count: 1
schemes:
- description: '`Authorization: Bearer ak_...`. See /docs/api/keys.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/antwork-io-openapi.json
  type: http
slug: antwork-io-authentication
source_filename: antwork-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/antwork-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: '`Authorization: Bearer ak_...`. See /docs/api/keys.'\n  sources:\n  - openapi/antwork-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/antwork-io/authentication/antwork-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Social Media
- Automation
- Scheduler
- Marketing
---
