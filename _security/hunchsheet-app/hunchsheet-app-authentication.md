---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hunchsheet-app-ask-api-openapi.yml
  format: yaml
  label: Hunch Ask API
  slug: hunchsheet-app-ask-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunchsheet-app/openapi/hunchsheet-app-ask-api-openapi.yml
- filename: hunchsheet-app-balance-api-openapi.yml
  format: yaml
  label: Hunch Balance API
  slug: hunchsheet-app-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunchsheet-app/openapi/hunchsheet-app-balance-api-openapi.yml
- filename: hunchsheet-app-checkout-api-openapi.yml
  format: yaml
  label: Hunch Checkout API
  slug: hunchsheet-app-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunchsheet-app/openapi/hunchsheet-app-checkout-api-openapi.yml
- filename: hunchsheet-app-quote-api-openapi.yml
  format: yaml
  label: Hunch Quote API
  slug: hunchsheet-app-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunchsheet-app/openapi/hunchsheet-app-quote-api-openapi.yml
- filename: hunchsheet-app-trial-api-openapi.yml
  format: yaml
  label: Hunch Trial API
  slug: hunchsheet-app-trial-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hunchsheet-app/openapi/hunchsheet-app-trial-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hunch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hunch secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hunch
provider_slug: hunchsheet-app
scheme_count: 1
schemes:
- bearerFormat: hunch_<40 hex characters>
  description: A Hunch key. Get 100 free rows with POST /trial {"source":"agent"}.
  name: hunchKey
  scheme: bearer
  sources:
  - openapi/hunchsheet-app-openapi.json
  type: http
slug: hunchsheet-app-authentication
source_filename: hunchsheet-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hunchsheet-app-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: hunchKey\n  type: http\n  scheme: bearer\n  bearerFormat: hunch_<40 hex characters>\n  description: A Hunch key. Get 100 free rows with POST /trial {\"source\":\"agent\"}.\n  sources:\n  - openapi/hunchsheet-app-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hunchsheet-app/authentication/hunchsheet-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Spreadsheets
- Productivity
- Software-as-a-Service
- Automation
- Company
---
