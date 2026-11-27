---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: anthid-com-account-manual-controls-api-openapi.yml
  format: yaml
  label: anthid-com Account Manual Controls API
  slug: anthid-com-account-manual-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-account-manual-controls-api-openapi.yml
- filename: anthid-com-account-risk-controls-api-openapi.yml
  format: yaml
  label: anthid-com Account Risk Controls API
  slug: anthid-com-account-risk-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-account-risk-controls-api-openapi.yml
- filename: anthid-com-account-time-controls-api-openapi.yml
  format: yaml
  label: anthid-com Account Time Controls API
  slug: anthid-com-account-time-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-account-time-controls-api-openapi.yml
- filename: anthid-com-control-evaluation-api-openapi.yml
  format: yaml
  label: anthid-com Control Evaluation API
  slug: anthid-com-control-evaluation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-control-evaluation-api-openapi.yml
- filename: anthid-com-effective-controls-api-openapi.yml
  format: yaml
  label: anthid-com Effective Controls API
  slug: anthid-com-effective-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-effective-controls-api-openapi.yml
- filename: anthid-com-organization-controls-api-openapi.yml
  format: yaml
  label: anthid-com Organization Controls API
  slug: anthid-com-organization-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-organization-controls-api-openapi.yml
- filename: anthid-com-symbol-manual-controls-api-openapi.yml
  format: yaml
  label: anthid-com Symbol Manual Controls API
  slug: anthid-com-symbol-manual-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-symbol-manual-controls-api-openapi.yml
- filename: anthid-com-symbol-risk-controls-api-openapi.yml
  format: yaml
  label: anthid-com Symbol Risk Controls API
  slug: anthid-com-symbol-risk-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-symbol-risk-controls-api-openapi.yml
- filename: anthid-com-symbol-time-controls-api-openapi.yml
  format: yaml
  label: anthid-com Symbol Time Controls API
  slug: anthid-com-symbol-time-controls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anthid-com/openapi/anthid-com-symbol-time-controls-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: anthid-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: anthid-com secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: anthid-com
provider_slug: anthid-com
scheme_count: 2
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/controls.json
  type: apiKey
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/controls.json
  type: http
slug: anthid-com-authentication
source_filename: anthid-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/controls.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/controls.json\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/controls.json\n"
source_yaml_url: https://artifacts.apis.io/anthid-com/authentication/anthid-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
---
