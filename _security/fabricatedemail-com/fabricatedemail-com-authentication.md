---
anonymous_access: false
api_key_in: []
api_specs:
- filename: fabricatedemail-com-health-api-openapi.yml
  format: yaml
  label: fabricatedemail-com Health API
  slug: fabricatedemail-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-health-api-openapi.yml
- filename: fabricatedemail-com-mcp-api-openapi.yml
  format: yaml
  label: fabricatedemail-com MCP API
  slug: fabricatedemail-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-mcp-api-openapi.yml
- filename: fabricatedemail-com-messages-api-openapi.yml
  format: yaml
  label: fabricatedemail-com Messages API
  slug: fabricatedemail-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-messages-api-openapi.yml
- filename: fabricatedemail-com-subscriptions-api-openapi.yml
  format: yaml
  label: fabricatedemail-com Subscriptions API
  slug: fabricatedemail-com-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabricatedemail-com/openapi/fabricatedemail-com-subscriptions-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fabricatedemail Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: fabricatedemail-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: fabricatedemail-com
provider_slug: fabricatedemail-com
scheme_count: 1
schemes:
- description: 'API key as a 64-hex character token, sent as `Authorization: Bearer <key>`'
  in: header
  name: Authorization
  type: bearer
slug: fabricatedemail-com-authentication
source_filename: fabricatedemail-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://fabricatedemail.com/docs/\nschemes:\n  - type: bearer\n    name: Authorization\n    in: header\n    description: \"API key as a 64-hex character token, sent as `Authorization: Bearer <key>`\"\n"
source_yaml_url: https://artifacts.apis.io/fabricatedemail-com/authentication/fabricatedemail-com-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Disposable
- Testing
- API
- Automation
- Service
---
