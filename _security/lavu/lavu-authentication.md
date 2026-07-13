---
api_key_in:
- query
api_specs:
- filename: lavu-poslavu-api.yml
  format: yaml
  label: Lavu (POSLavu) API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lavu/refs/heads/main/openapi/lavu-poslavu-api.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lavu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lavu secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Lavu
provider_slug: lavu
scheme_count: 1
schemes:
- description: POSLavu requests are authenticated with three form-encoded credentials (`dataname`, `key`, `token`) issued in the API tab of the POSLavu Control Panel. OpenAPI cannot express a multi-field credential as a single scheme; the `token` field is declared here as the representative credential and all three are required on every request.
  in: query
  name: posLavuCredentials
  parameter: token
  sources:
  - openapi/lavu-poslavu-api.yml
  type: apiKey
slug: lavu-authentication
source_filename: lavu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lavu-poslavu-api.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: posLavuCredentials\n  type: apiKey\n  in: query\n  parameter: token\n  description: POSLavu requests are authenticated with three form-encoded credentials (`dataname`,\n    `key`, `token`) issued in the API tab of the POSLavu Control Panel. OpenAPI cannot express\n    a multi-field credential as a single scheme; the `token` field is declared here as the representative\n    credential and all three are required on every request.\n  sources:\n  - openapi/lavu-poslavu-api.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lavu/refs/heads/main/authentication/lavu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Restaurant
- Point of Sale
- Payments
- Inventory
- Menu Management
---
