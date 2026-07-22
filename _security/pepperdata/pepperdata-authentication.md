---
api_key_in:
- header
api_specs:
- filename: pepperdata-rest-api-openapi.yml
  format: yaml
  label: Pepperdata REST API
  slug: pepperdata-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pepperdata/refs/heads/main/openapi/pepperdata-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Pepperdata Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pepperdata secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pepperdata
provider_slug: pepperdata
scheme_count: 1
schemes:
- description: 'API key authentication. Send the header `Authorization: PDAPI <API-key-id>:<API-key-token>`. Obtain a key at https://dashboard.pepperdata.com/account/apikeys and click Create API Key. A key is reusable until deleted or revoked.'
  in: header
  name: PDAPIAuth
  parameter: Authorization
  sources:
  - openapi/pepperdata-rest-api-openapi.yml
  type: apiKey
slug: pepperdata-authentication
source_filename: pepperdata-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/pepperdata-rest-api-openapi.yml\ndocs: https://docs.pepperdata.com/rest-api/00-common-api/\nnotes: >-\n  API key auth. Keys are created at https://dashboard.pepperdata.com/account/apikeys\n  (Create API Key) and sent in the Authorization header with the custom PDAPI scheme:\n  `Authorization: PDAPI <API-key-id>:<API-key-token>`. Keys are reusable until deleted\n  or revoked. All requests are HTTPS (TLS 1.2+).\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: PDAPIAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API key authentication. Send the header `Authorization: PDAPI <API-key-id>:<API-key-token>`.\n    Obtain a key at https://dashboard.pepperdata.com/account/apikeys and click Create API Key.\n    A key is reusable until deleted or revoked.'\n  sources:\n  - openapi/pepperdata-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pepperdata/refs/heads/main/authentication/pepperdata-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Observability
- Monitoring
- Kubernetes
- Big Data
- Cost Optimization
- Metrics
- APM
---
