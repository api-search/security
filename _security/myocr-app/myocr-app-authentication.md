---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: myocr-app-convert-api-openapi.yml
  format: yaml
  label: MyOCR Convert API
  slug: myocr-app-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myocr-app/openapi/myocr-app-convert-api-openapi.yml
- filename: myocr-app-jobs-api-openapi.yml
  format: yaml
  label: MyOCR Jobs API
  slug: myocr-app-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myocr-app/openapi/myocr-app-jobs-api-openapi.yml
- filename: myocr-app-keys-api-openapi.yml
  format: yaml
  label: MyOCR Keys API
  slug: myocr-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myocr-app/openapi/myocr-app-keys-api-openapi.yml
- filename: myocr-app-status-api-openapi.yml
  format: yaml
  label: MyOCR Status API
  slug: myocr-app-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/myocr-app/openapi/myocr-app-status-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MyOCR Authentication
name_suffix: Authentication
oauth_flows: []
overview: MyOCR secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MyOCR
provider_slug: myocr-app
scheme_count: 1
schemes:
- description: Send your API key in the `X-API-Key` header. Get one at /account/api.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/myocr-app-openapi.yml
  type: apiKey
slug: myocr-app-authentication
source_filename: myocr-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/myocr-app-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Send your API key in the `X-API-Key` header. Get one at /account/api.\n  sources:\n  - openapi/myocr-app-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/myocr-app/authentication/myocr-app-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- OCR
- Document Conversion
- Excel Export
- Finance
- Accounting
---
