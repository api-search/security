---
anonymous_access: false
api_key_in: []
api_specs:
- filename: pagecritic-app-audit-api-openapi.yml
  format: yaml
  label: PageCritic Audit API
  slug: pagecritic-app-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecritic-app/openapi/pagecritic-app-audit-api-openapi.yml
- filename: pagecritic-app-credits-api-openapi.yml
  format: yaml
  label: PageCritic Credits API
  slug: pagecritic-app-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecritic-app/openapi/pagecritic-app-credits-api-openapi.yml
- filename: pagecritic-app-keys-api-openapi.yml
  format: yaml
  label: PageCritic Keys API
  slug: pagecritic-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecritic-app/openapi/pagecritic-app-keys-api-openapi.yml
- filename: pagecritic-app-readiness-api-openapi.yml
  format: yaml
  label: PageCritic Readiness API
  slug: pagecritic-app-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecritic-app/openapi/pagecritic-app-readiness-api-openapi.yml
- filename: pagecritic-app-recheck-api-openapi.yml
  format: yaml
  label: PageCritic Recheck API
  slug: pagecritic-app-recheck-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagecritic-app/openapi/pagecritic-app-recheck-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: PageCritic Authentication
name_suffix: Authentication
oauth_flows: []
overview: PageCritic secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PageCritic
provider_slug: pagecritic-app
scheme_count: 1
schemes:
- description: Optional. Free from POST /api/v1/keys. With credits, audits return the full report.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/pagecritic-app-openapi.json
  type: http
slug: pagecritic-app-authentication
source_filename: pagecritic-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: derived\nsource: openapi/pagecritic-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Optional. Free from POST /api/v1/keys. With credits, audits return the full report.\n  sources:\n  - openapi/pagecritic-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/pagecritic-app/authentication/pagecritic-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Landing Pages
- Audit
- Software-as-a-Service
---
