---
api_key_in:
- header
- body
api_specs:
- filename: metrilo-tracking-openapi.yml
  format: yaml
  label: Metrilo Tracking & CRM API
  slug: metrilo-tracking-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/openapi/metrilo-tracking-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Metrilo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metrilo secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Metrilo
provider_slug: metrilo
scheme_count: 2
schemes:
- algorithm: HMAC-SHA256
  in: header
  key: API Secret
  message: raw JSON request body
  name: xDigest
  parameter: X-Digest
  required_for: all backend endpoints except POST /customer
  sources:
  - openapi/metrilo-tracking-openapi.yml
  type: apiKey
- in: body
  name: token
  parameter: token
  required_for: all requests
  sources:
  - openapi/metrilo-tracking-openapi.yml
  type: apiKey
slug: metrilo-authentication
source_filename: metrilo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://github.com/Metrilo/custom-integration\ndocs: https://github.com/Metrilo/custom-integration\nsummary:\n  types: [apiKey]\n  api_key_in: [header, body]\n  oauth2_flows: []\n  note: >-\n    Metrilo uses project-scoped credentials (API Token + API Secret) obtained\n    from Settings -> Installation. Requests carry the API Token in the JSON\n    body; every backend endpoint except POST /customer additionally requires an\n    X-Digest header holding an HMAC-SHA256 of the raw request body keyed with\n    the API Secret. There is no OAuth surface.\ncredentials:\n  - name: API Token\n    where: request body field `token`\n    obtained_from: Settings -> Installation (per project)\n  - name: API Secret\n    where: HMAC key for the X-Digest header (never transmitted)\n    obtained_from: Settings -> Installation (per project)\nschemes:\n  - name: xDigest\n    type: apiKey\n    in: header\n    parameter: X-Digest\n    algorithm:\
  \ HMAC-SHA256\n    message: raw JSON request body\n    key: API Secret\n    required_for: all backend endpoints except POST /customer\n    sources: [openapi/metrilo-tracking-openapi.yml]\n  - name: token\n    type: apiKey\n    in: body\n    parameter: token\n    required_for: all requests\n    sources: [openapi/metrilo-tracking-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metrilo/refs/heads/main/authentication/metrilo-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Ecommerce
- Analytics
- CRM
- Email Marketing
- Customer Retention
- Tracking
- Marketing
---
