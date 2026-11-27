---
anonymous_access: false
api_key_in: []
api_specs:
- filename: datanem-com-extraction-api-openapi.yml
  format: yaml
  label: Datanem Extraction API
  slug: datanem-com-extraction-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datanem-com/openapi/datanem-com-extraction-api-openapi.yml
- filename: datanem-com-templates-api-openapi.yml
  format: yaml
  label: Datanem Templates API
  slug: datanem-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datanem-com/openapi/datanem-com-templates-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Datanem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Datanem secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Datanem
provider_slug: datanem-com
scheme_count: 1
schemes:
- description: 'An API key from https://datanem.com/app/api, sent as `Authorization: Bearer <key>`. Available on ...'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/datanem-com-openapi.json
  type: http
slug: datanem-com-authentication
source_filename: datanem-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/datanem-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An API key from https://datanem.com/app/api, sent as `Authorization: Bearer\n    <key>`. Available on ...'\n  sources:\n  - openapi/datanem-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/datanem-com/authentication/datanem-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Extraction
- OCR
- Document Processing
- Spreadsheet Export
- United Kingdom
---
