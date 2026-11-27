---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: truelist-io-batch-email-validation-api-openapi.yml
  format: yaml
  label: Truelist Batch email validation API
  slug: truelist-io-batch-email-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truelist-io/openapi/truelist-io-batch-email-validation-api-openapi.yml
- filename: truelist-io-me-api-openapi.yml
  format: yaml
  label: Truelist Me API
  slug: truelist-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truelist-io/openapi/truelist-io-me-api-openapi.yml
- filename: truelist-io-retrieving-results-api-openapi.yml
  format: yaml
  label: Truelist Retrieving results API
  slug: truelist-io-retrieving-results-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truelist-io/openapi/truelist-io-retrieving-results-api-openapi.yml
- filename: truelist-io-single-email-validation-api-openapi.yml
  format: yaml
  label: Truelist Single email validation API
  slug: truelist-io-single-email-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/truelist-io/openapi/truelist-io-single-email-validation-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Truelist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truelist secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Truelist
provider_slug: truelist-io
scheme_count: 1
schemes:
- description: The user's bearer token sent via an Authorization header
  in: header
  name: truelist_auth
  parameter: Authorization
  sources:
  - openapi/truelist-io-openapi.yml
  type: apiKey
slug: truelist-io-authentication
source_filename: truelist-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: derived\nsource: openapi/truelist-io-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: truelist_auth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: The user's bearer token sent via an Authorization header\n  sources:\n  - openapi/truelist-io-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/truelist-io/authentication/truelist-io-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email Validation
- API
- SaaS
- Data Quality
- Marketing
---
