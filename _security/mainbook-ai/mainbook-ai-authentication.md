---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mainbook-ai-developer-api-openapi.yml
  format: yaml
  label: MainBook Developer API
  slug: mainbook-ai-developer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mainbook-ai/openapi/mainbook-ai-developer-api-openapi.yml
- filename: mainbook-ai-device-authorization-api-openapi.yml
  format: yaml
  label: MainBook Device Authorization API
  slug: mainbook-ai-device-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mainbook-ai/openapi/mainbook-ai-device-authorization-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MainBook Authentication
name_suffix: Authentication
oauth_flows: []
overview: MainBook secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MainBook
provider_slug: mainbook-ai
scheme_count: 1
schemes:
- description: 'API key `mb_live_…` in the Authorization header: `Authorization: Bearer mb_live_…`. Created in Settings → API.'
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/mainbook-ai-openapi.yml
  type: http
slug: mainbook-ai-authentication
source_filename: mainbook-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/mainbook-ai-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: 'API key `mb_live_…` in the Authorization header: `Authorization: Bearer mb_live_…`.\n    Created in Settings → API.'\n  sources:\n  - openapi/mainbook-ai-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/mainbook-ai/authentication/mainbook-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Bank Statement Conversion
- PDF to Excel
- Data Extraction
- Financial Data Processing
---
