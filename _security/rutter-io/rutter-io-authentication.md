---
api_key_in: []
api_specs:
- filename: rutter-io-openapi.yml
  format: yaml
  label: Rutter Connections API
  slug: rutter-io-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/openapi/rutter-io-openapi.yml
- filename: rutter-io-openapi.yml
  format: yaml
  label: Rutter Accounting API
  slug: rutter-io-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/openapi/rutter-io-openapi.yml
- filename: rutter-io-openapi.yml
  format: yaml
  label: Rutter Commerce API
  slug: rutter-io-commerce-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/openapi/rutter-io-openapi.yml
- filename: rutter-io-openapi.yml
  format: yaml
  label: Rutter Payments API
  slug: rutter-io-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/openapi/rutter-io-openapi.yml
- filename: rutter-io-openapi.yml
  format: yaml
  label: Rutter Webhooks API
  slug: rutter-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/openapi/rutter-io-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rutter Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rutter secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rutter
provider_slug: rutter-io
scheme_count: 1
schemes:
- description: HTTP Basic auth. Username is your Rutter client_id, password is your Rutter secret. Requests must also include the `X-Rutter-Version` header and, for data endpoints, the `access_token` query parameter.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/rutter-io-openapi.yml
  type: http
slug: rutter-io-authentication
source_filename: rutter-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rutter-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth. Username is your Rutter client_id, password is your Rutter secret.\n    Requests must also include the `X-Rutter-Version` header and, for data endpoints, the `access_token`\n    query parameter.\n  sources:\n  - openapi/rutter-io-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rutter-io/refs/heads/main/authentication/rutter-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Unified API
- Accounting
- Commerce
- Payments
- Business Data
- Integrations
---
