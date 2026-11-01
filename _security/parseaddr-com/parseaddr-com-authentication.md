---
anonymous_access: false
api_key_in: []
api_specs:
- filename: parseaddr-com-checkout-api-openapi.yml
  format: yaml
  label: parseaddr-com Checkout API
  slug: parseaddr-com-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-checkout-api-openapi.yml
- filename: parseaddr-com-credits-api-openapi.yml
  format: yaml
  label: parseaddr-com Credits API
  slug: parseaddr-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-credits-api-openapi.yml
- filename: parseaddr-com-expand-api-openapi.yml
  format: yaml
  label: parseaddr-com Expand API
  slug: parseaddr-com-expand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-expand-api-openapi.yml
- filename: parseaddr-com-health-api-openapi.yml
  format: yaml
  label: parseaddr-com Health API
  slug: parseaddr-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-health-api-openapi.yml
- filename: parseaddr-com-parse-api-openapi.yml
  format: yaml
  label: parseaddr-com Parse API
  slug: parseaddr-com-parse-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-parse-api-openapi.yml
- filename: parseaddr-com-signup-api-openapi.yml
  format: yaml
  label: parseaddr-com Signup API
  slug: parseaddr-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-signup-api-openapi.yml
- filename: parseaddr-com-usage-api-openapi.yml
  format: yaml
  label: parseaddr-com Usage API
  slug: parseaddr-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/parseaddr-com/openapi/parseaddr-com-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Parseaddr Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: parseaddr-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: parseaddr-com
provider_slug: parseaddr-com
scheme_count: 1
schemes:
- description: 'Your parseaddr API key as a Bearer token (Authorization: Bearer pa_live_…).'
  name: ApiKeyBearer
  scheme: bearer
  sources:
  - openapi/api-parseaddr-com-openapi.json
  - openapi/parseaddr-com-openapi.json
  type: http
slug: parseaddr-com-authentication
source_filename: parseaddr-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: derived\nsource: openapi/api-parseaddr-com-openapi.json, openapi/parseaddr-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyBearer\n  type: http\n  scheme: bearer\n  description: 'Your parseaddr API key as a Bearer token (Authorization: Bearer pa_live_…).'\n  sources:\n  - openapi/api-parseaddr-com-openapi.json\n  - openapi/parseaddr-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/parseaddr-com/authentication/parseaddr-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Address
- Parsing
- API
- libpostal
---
