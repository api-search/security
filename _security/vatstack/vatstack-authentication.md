---
api_key_in:
- header
api_specs:
- filename: vatstack-batches-api-openapi.yml
  format: yaml
  label: Vatstack Batches API
  slug: vatstack-batches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-batches-api-openapi.yml
- filename: vatstack-evidences-api-openapi.yml
  format: yaml
  label: Vatstack Evidences API
  slug: vatstack-evidences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-evidences-api-openapi.yml
- filename: vatstack-hits-api-openapi.yml
  format: yaml
  label: Vatstack Hits API
  slug: vatstack-hits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-hits-api-openapi.yml
- filename: vatstack-quotes-api-openapi.yml
  format: yaml
  label: Vatstack Quotes API
  slug: vatstack-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-quotes-api-openapi.yml
- filename: vatstack-rates-api-openapi.yml
  format: yaml
  label: Vatstack Rates API
  slug: vatstack-rates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-rates-api-openapi.yml
- filename: vatstack-supplies-api-openapi.yml
  format: yaml
  label: Vatstack Supplies API
  slug: vatstack-supplies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-supplies-api-openapi.yml
- filename: vatstack-validations-api-openapi.yml
  format: yaml
  label: Vatstack Validations API
  slug: vatstack-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/openapi/vatstack-validations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vatstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vatstack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vatstack
provider_slug: vatstack
scheme_count: 1
schemes:
- in: header
  name: publicKey
  parameter: X-API-KEY
  sources:
  - openapi/vatstack-openapi.json
  type: apiKey
slug: vatstack-authentication
source_filename: vatstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vatstack-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: publicKey\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/vatstack-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vatstack/refs/heads/main/authentication/vatstack-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- VAT
- Tax
- Validation
- EU
- Europe
- Compliance
- Finance
- Business
---
