---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fallax-io-campaigns-api-openapi.yml
  format: yaml
  label: Fallax Campaigns API
  slug: fallax-io-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-campaigns-api-openapi.yml
- filename: fallax-io-events-api-openapi.yml
  format: yaml
  label: Fallax Events API
  slug: fallax-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-events-api-openapi.yml
- filename: fallax-io-me-api-openapi.yml
  format: yaml
  label: Fallax Me API
  slug: fallax-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-me-api-openapi.yml
- filename: fallax-io-people-api-openapi.yml
  format: yaml
  label: Fallax People API
  slug: fallax-io-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-people-api-openapi.yml
- filename: fallax-io-reports-api-openapi.yml
  format: yaml
  label: Fallax Reports API
  slug: fallax-io-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-reports-api-openapi.yml
- filename: fallax-io-summary-api-openapi.yml
  format: yaml
  label: Fallax Summary API
  slug: fallax-io-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fallax-io/openapi/fallax-io-summary-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Fallax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fallax secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fallax
provider_slug: fallax-io
scheme_count: 1
schemes:
- bearerFormat: flx_
  description: A workspace API key, created in Settings.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fallax-io-openapi.json
  type: http
slug: fallax-io-authentication
source_filename: fallax-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/fallax-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: flx_\n  description: A workspace API key, created in Settings.\n  sources:\n  - openapi/fallax-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/fallax-io/authentication/fallax-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Awareness
- Phishing
- Compliance
- Software-as-a-Service
- Company
---
