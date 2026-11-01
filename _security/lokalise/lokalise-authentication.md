---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: lokalise-files-api-openapi.yml
  format: yaml
  label: Lokalise Files API
  slug: lokalise-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lokalise/openapi/lokalise-files-api-openapi.yml
- filename: lokalise-keys-api-openapi.yml
  format: yaml
  label: Lokalise Keys API
  slug: lokalise-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lokalise/openapi/lokalise-keys-api-openapi.yml
- filename: lokalise-projects-api-openapi.yml
  format: yaml
  label: Lokalise Projects API
  slug: lokalise-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lokalise/openapi/lokalise-projects-api-openapi.yml
- filename: lokalise-branches-api-openapi.yml
  format: yaml
  label: Lokalise Branches API
  slug: lokalise-branches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lokalise/openapi/lokalise-branches-api-openapi.yml
- filename: lokalise-comments-api-openapi.yml
  format: yaml
  label: Lokalise Comments API
  slug: lokalise-comments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lokalise/openapi/lokalise-comments-api-openapi.yml
- filename: lokalise-languages-api-openapi.yml
  format: yaml
  label: Lokalise Languages API
  slug: lokalise-languages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lokalise/openapi/lokalise-languages-api-openapi.yml
- filename: lokalise-queued-processes-api-openapi.yml
  format: yaml
  label: Lokalise Queued Processes API
  slug: lokalise-queued-processes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lokalise/openapi/lokalise-queued-processes-api-openapi.yml
- filename: lokalise-screenshots-api-openapi.yml
  format: yaml
  label: Lokalise Screenshots API
  slug: lokalise-screenshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lokalise/openapi/lokalise-screenshots-api-openapi.yml
- filename: lokalise-tasks-api-openapi.yml
  format: yaml
  label: Lokalise Tasks API
  slug: lokalise-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lokalise/openapi/lokalise-tasks-api-openapi.yml
- filename: lokalise-translations-api-openapi.yml
  format: yaml
  label: Lokalise Translations API
  slug: lokalise-translations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lokalise/openapi/lokalise-translations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Lokalise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lokalise secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lokalise
provider_slug: lokalise
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Token
  sources:
  - openapi/lokalise-openapi.yml
  type: apiKey
slug: lokalise-authentication
source_filename: lokalise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lokalise-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Token\n  sources:\n  - openapi/lokalise-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/lokalise/authentication/lokalise-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Localization
- Translation
- TMS
- AI Machine Translation
- REST
- Developer Tools
---
