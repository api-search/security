---
anonymous_access: false
api_key_in: []
api_specs:
- filename: evidujzdarma-cz-account-api-openapi.yml
  format: yaml
  label: EvidujZdarma Account API
  slug: evidujzdarma-cz-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-account-api-openapi.yml
- filename: evidujzdarma-cz-closings-api-openapi.yml
  format: yaml
  label: EvidujZdarma Closings API
  slug: evidujzdarma-cz-closings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-closings-api-openapi.yml
- filename: evidujzdarma-cz-oauth-api-openapi.yml
  format: yaml
  label: EvidujZdarma OAuth API
  slug: evidujzdarma-cz-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-oauth-api-openapi.yml
- filename: evidujzdarma-cz-sales-api-openapi.yml
  format: yaml
  label: EvidujZdarma Sales API
  slug: evidujzdarma-cz-sales-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-sales-api-openapi.yml
- filename: evidujzdarma-cz-units-api-openapi.yml
  format: yaml
  label: EvidujZdarma Units API
  slug: evidujzdarma-cz-units-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-units-api-openapi.yml
- filename: evidujzdarma-cz-webhooks-api-openapi.yml
  format: yaml
  label: EvidujZdarma Webhooks API
  slug: evidujzdarma-cz-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/evidujzdarma-cz/openapi/evidujzdarma-cz-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: EvidujZdarma Authentication
name_suffix: Authentication
oauth_flows: []
overview: EvidujZdarma secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: EvidujZdarma
provider_slug: evidujzdarma-cz
scheme_count: 1
schemes:
- description: Integration token ezk_test_… (Playground) or ezk_live_… (production).
  name: bearer
  scheme: bearer
  sources:
  - openapi/evidujzdarma-cz-openapi.json
  type: http
slug: evidujzdarma-cz-authentication
source_filename: evidujzdarma-cz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: derived\nsource: openapi/evidujzdarma-cz-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Integration token ezk_test_… (Playground) or ezk_live_… (production).\n  sources:\n  - openapi/evidujzdarma-cz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/evidujzdarma-cz/authentication/evidujzdarma-cz-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Czech Republic
- EET
---
