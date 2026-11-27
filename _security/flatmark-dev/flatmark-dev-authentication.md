---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: flatmark-dev-account-api-openapi.yml
  format: yaml
  label: flatmark Account API
  slug: flatmark-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatmark-dev/openapi/flatmark-dev-account-api-openapi.yml
- filename: flatmark-dev-convert-api-openapi.yml
  format: yaml
  label: flatmark Convert API
  slug: flatmark-dev-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatmark-dev/openapi/flatmark-dev-convert-api-openapi.yml
- filename: flatmark-dev-jobs-api-openapi.yml
  format: yaml
  label: flatmark Jobs API
  slug: flatmark-dev-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatmark-dev/openapi/flatmark-dev-jobs-api-openapi.yml
- filename: flatmark-dev-webhooks-api-openapi.yml
  format: yaml
  label: flatmark Webhooks API
  slug: flatmark-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/flatmark-dev/openapi/flatmark-dev-webhooks-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: flatmark Authentication
name_suffix: Authentication
oauth_flows: []
overview: flatmark secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: flatmark
provider_slug: flatmark-dev
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/flatmark-dev-openapi.json
  type: apiKey
slug: flatmark-dev-authentication
source_filename: flatmark-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/flatmark-dev-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/flatmark-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/flatmark-dev/authentication/flatmark-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- PDF
- Markdown
- Conversion
- RAG
---
