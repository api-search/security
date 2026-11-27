---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: imperioutils-com-demo-pubblica-api-openapi.yml
  format: yaml
  label: Imperio Demo pubblica API
  slug: imperioutils-com-demo-pubblica-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-demo-pubblica-api-openapi.yml
- filename: imperioutils-com-health-api-openapi.yml
  format: yaml
  label: Imperio Health API
  slug: imperioutils-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-health-api-openapi.yml
- filename: imperioutils-com-mcp-api-openapi.yml
  format: yaml
  label: Imperio MCP API
  slug: imperioutils-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-mcp-api-openapi.yml
- filename: imperioutils-com-registry-api-openapi.yml
  format: yaml
  label: Imperio Registry API
  slug: imperioutils-com-registry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-registry-api-openapi.yml
- filename: imperioutils-com-tool-api-openapi.yml
  format: yaml
  label: Imperio Tool API
  slug: imperioutils-com-tool-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-tool-api-openapi.yml
- filename: imperioutils-com-webhookcapture-api-openapi.yml
  format: yaml
  label: Imperio Webhook Capture API
  slug: imperioutils-com-webhookcapture-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imperioutils-com/openapi/imperioutils-com-webhookcapture-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Imperio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Imperio secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Imperio
provider_slug: imperioutils-com
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: JWT
  scheme: bearer
  sources:
  - openapi/imperioutils-com-openapi.yml
  type: http
- in: header
  name: ApiKey
  parameter: X-API-Key
  sources:
  - openapi/imperioutils-com-openapi.yml
  type: apiKey
slug: imperioutils-com-authentication
source_filename: imperioutils-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/imperioutils-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/imperioutils-com-openapi.yml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/imperioutils-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/imperioutils-com/authentication/imperioutils-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Finance
- Tax
- Fraud Prevention
- Italy
---
