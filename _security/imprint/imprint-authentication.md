---
api_key_in: []
api_specs:
- filename: imprint-openapi-original.yml
  format: yaml
  label: Imprint Public API
  slug: imprint-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/openapi/imprint-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Imprint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imprint secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Imprint
provider_slug: imprint
scheme_count: 2
schemes:
- description: 'Basic HTTP authentication. Allowed headers-- Authorization: Basic <base64(api_key_id:api_key_secret)>'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/imprint-openapi-original.yml
  type: http
- bearerFormat: auth-scheme
  description: 'Bearer HTTP authentication. Allowed headers-- Authorization: Bearer <api_key>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/imprint-openapi-original.yml
  type: http
slug: imprint-authentication
source_filename: imprint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/imprint-openapi-original.yml\ndocs: https://docs.imprint.co/authentication\nmodel: >-\n  API-key auth, environment-specific keys managed in the Imprint Dashboard.\n  Provide the API key as the HTTP Basic username (empty password), or as a Bearer\n  token. Multi-product partners target a co-branded product with the\n  x-imprint-merchant-key header.\nmulti_product_header:\n  name: x-imprint-merchant-key\n  required: false\nkey_management:\n  create: POST /v2/keys (createKey)\n  delete: DELETE /v2/keys (deleteKey)\n  rotation_docs: https://docs.imprint.co/api-key-rotation\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'Basic HTTP authentication. Allowed headers-- Authorization: Basic <base64(api_key_id:api_key_secret)>'\n  sources:\n  - openapi/imprint-openapi-original.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: auth-scheme\n  description:\
  \ 'Bearer HTTP authentication. Allowed headers-- Authorization: Bearer <api_key>'\n  sources:\n  - openapi/imprint-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imprint/refs/heads/main/authentication/imprint-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Financial Services
- Fintech
- Credit Cards
- Co-Branded Cards
- Payments
- Loans
- Rewards
- Loyalty
- Embedded Finance
---
