---
api_key_in:
- header
api_specs:
- filename: docsumo-openapi.yml
  format: yaml
  label: Docsumo Documents & Extraction API
  slug: docsumo-documents-extraction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/openapi/docsumo-openapi.yml
- filename: docsumo-openapi.yml
  format: yaml
  label: Docsumo Document Types API
  slug: docsumo-document-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/openapi/docsumo-openapi.yml
- filename: docsumo-openapi.yml
  format: yaml
  label: Docsumo Review & Validation API
  slug: docsumo-review-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/openapi/docsumo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Docsumo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Docsumo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Docsumo
provider_slug: docsumo
scheme_count: 1
schemes:
- description: Personal API key from https://app.docsumo.com/settings/webhook-api/. Also accepted as the `X-API-KEY` header.
  in: header
  name: apiKeyAuth
  parameter: apikey
  sources:
  - openapi/docsumo-openapi.yml
  type: apiKey
slug: docsumo-authentication
source_filename: docsumo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/docsumo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: apikey\n  description: Personal API key from https://app.docsumo.com/settings/webhook-api/. Also accepted\n    as the `X-API-KEY` header.\n  sources:\n  - openapi/docsumo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docsumo/refs/heads/main/authentication/docsumo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Document Processing
- IDP
- OCR
- Data Extraction
- AI
---
