---
anonymous_access: false
api_key_in: []
api_specs:
- filename: valotcg-analysis-api-openapi.yml
  format: yaml
  label: Valo.Data Analysis API
  slug: valotcg-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-analysis-api-openapi.yml
- filename: valotcg-cards-api-openapi.yml
  format: yaml
  label: Valo.Data Cards API
  slug: valotcg-cards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-cards-api-openapi.yml
- filename: valotcg-editions-api-openapi.yml
  format: yaml
  label: Valo.Data Editions API
  slug: valotcg-editions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-editions-api-openapi.yml
- filename: valotcg-games-api-openapi.yml
  format: yaml
  label: Valo.Data Games API
  slug: valotcg-games-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-games-api-openapi.yml
- filename: valotcg-sealed-api-openapi.yml
  format: yaml
  label: Valo.Data Sealed API
  slug: valotcg-sealed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-sealed-api-openapi.yml
- filename: valotcg-usage-api-openapi.yml
  format: yaml
  label: Valo.Data Usage API
  slug: valotcg-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/valotcg/openapi/valotcg-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Valotcg Authentication
name_suffix: Authentication
oauth_flows: []
overview: Valo.Data secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Valo.Data
provider_slug: valotcg
scheme_count: 1
schemes:
- description: '`Authorization: Bearer vd_live_…` (or `vd_test_…`). Keys are shown once at creation.'
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/valotcg-data-v1-openapi.json
  type: http
slug: valotcg-authentication
source_filename: valotcg-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/valotcg-data-v1-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  description: '`Authorization: Bearer vd_live_…` (or `vd_test_…`). Keys are shown once at creation.'\n  sources:\n  - openapi/valotcg-data-v1-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/valotcg/authentication/valotcg-authentication.yml
summary_line: http · 1 scheme
tags:
- Trading Card Games
- Pricing Data
- Vision
---
