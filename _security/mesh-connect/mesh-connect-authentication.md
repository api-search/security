---
api_key_in:
- header
api_specs:
- filename: mesh-connect-openapi-original.json
  format: json
  label: Mesh Connect Integration API
  slug: mesh-connect-integration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-openapi-original.json
- filename: mesh-connect-admin-openapi-original.json
  format: json
  label: Mesh Admin API
  slug: mesh-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/openapi/mesh-connect-admin-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mesh Connect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mesh Connect secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Mesh Connect
provider_slug: mesh-connect
scheme_count: 3
schemes:
- description: 'Authorization header using the Bearer scheme. Example: "Authorization: Bearer {Value}"'
  name: Bearer
  scheme: bearer
  sources:
  - openapi/mesh-connect-admin-openapi-original.json
  type: http
- description: Contact Mesh to get client Secret
  in: header
  name: Client-Secret
  parameter: X-Client-Secret
  sources:
  - openapi/mesh-connect-openapi-original.json
  type: apiKey
- description: Contact Mesh to get client Id
  in: header
  name: Client-Id
  parameter: X-Client-Id
  sources:
  - openapi/mesh-connect-openapi-original.json
  type: apiKey
slug: mesh-connect-authentication
source_filename: mesh-connect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mesh-connect-admin-openapi-original.json, openapi/mesh-connect-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: 'Authorization header using the Bearer scheme. Example: \"Authorization: Bearer\n    {Value}\"'\n  sources:\n  - openapi/mesh-connect-admin-openapi-original.json\n- name: Client-Secret\n  type: apiKey\n  in: header\n  parameter: X-Client-Secret\n  description: Contact Mesh to get client Secret\n  sources:\n  - openapi/mesh-connect-openapi-original.json\n- name: Client-Id\n  type: apiKey\n  in: header\n  parameter: X-Client-Id\n  description: Contact Mesh to get client Id\n  sources:\n  - openapi/mesh-connect-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mesh-connect/refs/heads/main/authentication/mesh-connect-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Crypto Infrastructure
- Crypto Payments
- Digital Assets
- Wallets
- Exchanges
- Embedded Finance
- Stablecoins
- Payments
---
