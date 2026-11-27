---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: invowerk-dev-account-api-openapi.yml
  format: yaml
  label: invowerk Account API
  slug: invowerk-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-account-api-openapi.yml
- filename: invowerk-dev-generation-api-openapi.yml
  format: yaml
  label: invowerk Generation API
  slug: invowerk-dev-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-generation-api-openapi.yml
- filename: invowerk-dev-rendering-api-openapi.yml
  format: yaml
  label: invowerk Rendering API
  slug: invowerk-dev-rendering-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-rendering-api-openapi.yml
- filename: invowerk-dev-rules-api-openapi.yml
  format: yaml
  label: invowerk Rules API
  slug: invowerk-dev-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-rules-api-openapi.yml
- filename: invowerk-dev-transform-api-openapi.yml
  format: yaml
  label: invowerk Transform API
  slug: invowerk-dev-transform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-transform-api-openapi.yml
- filename: invowerk-dev-validation-api-openapi.yml
  format: yaml
  label: invowerk Validation API
  slug: invowerk-dev-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/invowerk-dev/openapi/invowerk-dev-validation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: invowerk Authentication
name_suffix: Authentication
oauth_flows: []
overview: invowerk secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: invowerk
provider_slug: invowerk-dev
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/invowerk-dev-openapi.yml
  type: apiKey
slug: invowerk-dev-authentication
source_filename: invowerk-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/invowerk-dev-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/invowerk-dev-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/invowerk-dev/authentication/invowerk-dev-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Invoicing
- e-invoice
- PDF
- Germany
---
