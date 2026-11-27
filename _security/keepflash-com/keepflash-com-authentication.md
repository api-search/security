---
anonymous_access: false
api_key_in: []
api_specs:
- filename: keepflash-com-agent-authorization-api-openapi.yml
  format: yaml
  label: KeepFlash Agent authorization API
  slug: keepflash-com-agent-authorization-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepflash-com/openapi/keepflash-com-agent-authorization-api-openapi.yml
- filename: keepflash-com-mcp-api-openapi.yml
  format: yaml
  label: KeepFlash MCP API
  slug: keepflash-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/keepflash-com/openapi/keepflash-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: KeepFlash Authentication
name_suffix: Authentication
oauth_flows: []
overview: KeepFlash secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KeepFlash
provider_slug: keepflash-com
scheme_count: 1
schemes:
- bearerFormat: KeepFlash Agent Access token
  description: Token returned by the device-token operation.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/keepflash-com-openapi.yml
  type: http
slug: keepflash-com-authentication
source_filename: keepflash-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/keepflash-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: KeepFlash Agent Access token\n  description: Token returned by the device-token operation.\n  sources:\n  - openapi/keepflash-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/keepflash-com/authentication/keepflash-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Knowledge Management
- Personal Knowledge Library
- Productivity
- Search
---
