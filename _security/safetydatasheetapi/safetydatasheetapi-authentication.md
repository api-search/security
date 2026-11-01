---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: SDS/MSDS Extraction REST API
  slug: sdsmsds-extraction-rest-api
  spec_type: OpenAPI
  url: https://safetydatasheetapi.com/openapi.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Safetydatasheetapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Safety Data Sheet (SDS/MSDS) Extraction API secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Safety Data Sheet (SDS/MSDS) Extraction API
provider_slug: safetydatasheetapi
scheme_count: 2
schemes:
- bearerFormat: API Key
  description: 'API key sent as `Authorization: Bearer <api_key>`. Never send keys in the query string.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/safetydatasheetapi-openapi.yaml
  type: http
- description: Alternative to the Bearer header. Send the same API key as `X-API-Key`.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/safetydatasheetapi-openapi.yaml
  type: apiKey
slug: safetydatasheetapi-authentication
source_filename: safetydatasheetapi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: derived\nsource: openapi/safetydatasheetapi-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'API key sent as `Authorization: Bearer <api_key>`. Never send keys in the query\n    string.'\n  sources:\n  - openapi/safetydatasheetapi-openapi.yaml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Alternative to the Bearer header. Send the same API key as `X-API-Key`.\n  sources:\n  - openapi/safetydatasheetapi-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/safetydatasheetapi/authentication/safetydatasheetapi-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Safety Data Sheets
- msds
- ghs-classification
- chemical-compliance
- EHS
- Regulatory Compliance
- Document Extraction
- OCR
- pdf-to-json
- data-normalization
- ERP Integration
- PLM
- Supply Chain
- Chemicals
---
