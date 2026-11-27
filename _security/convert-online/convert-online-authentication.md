---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: convert-online-catalogue-api-openapi.yml
  format: yaml
  label: Convert.Online Catalogue API
  slug: convert-online-catalogue-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convert-online/openapi/convert-online-catalogue-api-openapi.yml
- filename: convert-online-downloads-api-openapi.yml
  format: yaml
  label: Convert.Online Downloads API
  slug: convert-online-downloads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convert-online/openapi/convert-online-downloads-api-openapi.yml
- filename: convert-online-imports-api-openapi.yml
  format: yaml
  label: Convert.Online Imports API
  slug: convert-online-imports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convert-online/openapi/convert-online-imports-api-openapi.yml
- filename: convert-online-jobs-api-openapi.yml
  format: yaml
  label: Convert.Online Jobs API
  slug: convert-online-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/convert-online/openapi/convert-online-jobs-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Convert.Online Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convert.Online secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Convert.Online
provider_slug: convert-online
scheme_count: 2
schemes:
- description: 'An API key from Dashboard → API Keys, sent as `Authorization: Bearer <key>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/convert-online-openapi.yml
  type: http
- description: The same key, sent in its own header instead.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/convert-online-openapi.yml
  type: apiKey
slug: convert-online-authentication
source_filename: convert-online-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://convert.online/api-docs\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An API key from Dashboard → API Keys, sent as `Authorization: Bearer\n    <key>`.'\n  sources:\n  - openapi/convert-online-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: The same key, sent in its own header instead.\n  sources:\n  - openapi/convert-online-openapi.yml\ndocs: https://convert.online/api-docs#authentication\nkey_management:\n  issued_at: Dashboard → API Keys\n  shown_once: true\n  storage_note: A key is shown once when you create it — store it securely; we only\n    keep a hash.\n  ip_restriction: If a key is restricted to specific IPs and the request comes from\n    another address, it returns 403.\nunauthenticated_status: 401\nunauthenticated_operations:\n- 'createJob (with \"\
  sandbox\": true only — docs: \"no API key is required\")'\n- downloadResult (token in path)\nwebhook_signing:\n  header: X-Convert-Signature\n  algorithm: HMAC-SHA256 of the raw body, hex, prefixed sha256=\n  secret: webhook signing secret from Dashboard → API Keys\n"
source_yaml_url: https://artifacts.apis.io/convert-online/authentication/convert-online-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- File Conversion
- Document Conversion
- Image Conversion
- Video Conversion
- Audio Conversion
- OCR
- MCP
---
