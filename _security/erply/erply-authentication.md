---
api_key_in:
- header
api_specs:
- filename: erply-pim-openapi.json
  format: json
  label: Erply PIM API
  slug: erply-pim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erply/refs/heads/main/openapi/erply-pim-openapi.json
- filename: erply-assignments-openapi.json
  format: json
  label: Erply Assignments API
  slug: erply-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erply/refs/heads/main/openapi/erply-assignments-openapi.json
- filename: erply-cafa-openapi.json
  format: json
  label: Erply CAFA API
  slug: erply-cafa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erply/refs/heads/main/openapi/erply-cafa-openapi.json
- filename: erply-webhook-openapi.json
  format: json
  label: Erply Webhook Manager API
  slug: erply-webhook-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/erply/refs/heads/main/openapi/erply-webhook-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Erply Authentication
name_suffix: Authentication
oauth_flows: []
overview: Erply secures its APIs with apiKey across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Erply
provider_slug: erply
scheme_count: 6
schemes:
- in: header
  name: AccessToken
  parameter: accessToken
  sources:
  - openapi/erply-assignments-openapi.json
  type: apiKey
- in: header
  name: ErplyClientCode
  parameter: clientCode
  sources:
  - openapi/erply-assignments-openapi.json
  - openapi/erply-cafa-openapi.json
  - openapi/erply-pim-openapi.json
  - openapi/erply-webhook-openapi.json
  type: apiKey
- in: header
  name: ErplyJWT
  parameter: jwt
  sources:
  - openapi/erply-assignments-openapi.json
  - openapi/erply-cafa-openapi.json
  - openapi/erply-pim-openapi.json
  type: apiKey
- in: header
  name: ErplySession
  parameter: sessionKey
  sources:
  - openapi/erply-assignments-openapi.json
  - openapi/erply-cafa-openapi.json
  - openapi/erply-pim-openapi.json
  - openapi/erply-webhook-openapi.json
  type: apiKey
- in: header
  name: RequestKey
  parameter: requestKey
  sources:
  - openapi/erply-assignments-openapi.json
  type: apiKey
- in: header
  name: hmac-auth
  parameter: hmac-auth
  sources:
  - openapi/erply-cafa-openapi.json
  type: apiKey
slug: erply-authentication
source_filename: erply-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/erply-assignments-openapi.json, openapi/erply-cafa-openapi.json, openapi/erply-pim-openapi.json,\n  openapi/erply-webhook-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AccessToken\n  type: apiKey\n  in: header\n  parameter: accessToken\n  sources:\n  - openapi/erply-assignments-openapi.json\n- name: ErplyClientCode\n  type: apiKey\n  in: header\n  parameter: clientCode\n  sources:\n  - openapi/erply-assignments-openapi.json\n  - openapi/erply-cafa-openapi.json\n  - openapi/erply-pim-openapi.json\n  - openapi/erply-webhook-openapi.json\n- name: ErplyJWT\n  type: apiKey\n  in: header\n  parameter: jwt\n  sources:\n  - openapi/erply-assignments-openapi.json\n  - openapi/erply-cafa-openapi.json\n  - openapi/erply-pim-openapi.json\n- name: ErplySession\n  type: apiKey\n  in: header\n  parameter: sessionKey\n  sources:\n  - openapi/erply-assignments-openapi.json\n  - openapi/erply-cafa-openapi.json\n\
  \  - openapi/erply-pim-openapi.json\n  - openapi/erply-webhook-openapi.json\n- name: RequestKey\n  type: apiKey\n  in: header\n  parameter: requestKey\n  sources:\n  - openapi/erply-assignments-openapi.json\n- name: hmac-auth\n  type: apiKey\n  in: header\n  parameter: hmac-auth\n  sources:\n  - openapi/erply-cafa-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/erply/refs/heads/main/authentication/erply-authentication.yml
summary_line: apiKey · 6 schemes
tags:
- Retail
- Point of Sale
- Inventory
- Product Information Management
- CRM
- Ecommerce
- Warehouse Management
- Webhooks
- Company
---
