---
anonymous_access: false
api_key_in: []
api_specs:
- filename: myoddly-com-action-cards-api-openapi.yml
  format: yaml
  label: oddly Action Cards API
  slug: myoddly-com-action-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myoddly-com/openapi/myoddly-com-action-cards-api-openapi.yml
- filename: myoddly-com-actions-api-openapi.yml
  format: yaml
  label: oddly Actions API
  slug: myoddly-com-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myoddly-com/openapi/myoddly-com-actions-api-openapi.yml
- filename: myoddly-com-benchmarks-api-openapi.yml
  format: yaml
  label: oddly Benchmarks API
  slug: myoddly-com-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myoddly-com/openapi/myoddly-com-benchmarks-api-openapi.yml
- filename: myoddly-com-channels-api-openapi.yml
  format: yaml
  label: oddly Channels API
  slug: myoddly-com-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myoddly-com/openapi/myoddly-com-channels-api-openapi.yml
- filename: myoddly-com-data-api-openapi.yml
  format: yaml
  label: oddly Data API
  slug: myoddly-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myoddly-com/openapi/myoddly-com-data-api-openapi.yml
- filename: myoddly-com-margins-api-openapi.yml
  format: yaml
  label: oddly Margins API
  slug: myoddly-com-margins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myoddly-com/openapi/myoddly-com-margins-api-openapi.yml
- filename: myoddly-com-playbooks-api-openapi.yml
  format: yaml
  label: oddly Playbooks API
  slug: myoddly-com-playbooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myoddly-com/openapi/myoddly-com-playbooks-api-openapi.yml
- filename: myoddly-com-prescriptions-api-openapi.yml
  format: yaml
  label: oddly Prescriptions API
  slug: myoddly-com-prescriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myoddly-com/openapi/myoddly-com-prescriptions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: oddly Authentication
name_suffix: Authentication
oauth_flows: []
overview: oddly secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: oddly
provider_slug: myoddly-com
scheme_count: 1
schemes:
- bearerFormat: oddly_live_*
  description: 'API key minted at /dashboard/developers. Send as: Authorization: Bearer oddly_live_...'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/myoddly-com-openapi.yml
  type: http
slug: myoddly-com-authentication
source_filename: myoddly-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/myoddly-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: oddly_live_*\n  description: 'API key minted at /dashboard/developers. Send as: Authorization: Bearer oddly_live_...'\n  sources:\n  - openapi/myoddly-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/myoddly-com/authentication/myoddly-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Verification
- Data Integrity
- Compliance
- Platform
---
