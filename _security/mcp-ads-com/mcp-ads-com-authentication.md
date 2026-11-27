---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mcp-ads-com-developer-api-openapi.yml
  format: yaml
  label: mcp-ads-com Developer API
  slug: mcp-ads-com-developer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mcp-ads-com/openapi/mcp-ads-com-developer-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: mcp-ads-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: mcp-ads-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: mcp-ads-com
provider_slug: mcp-ads-com
scheme_count: 1
schemes:
- description: An mcp_live_ key from the developer console.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/mcp-ads-com-openapi.json
  type: http
slug: mcp-ads-com-authentication
source_filename: mcp-ads-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: derived\nsource: openapi/mcp-ads-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: An mcp_live_ key from the developer console.\n  sources:\n  - openapi/mcp-ads-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mcp-ads-com/authentication/mcp-ads-com-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Assistant
- Marketing Automation
- Cross-Platform Ads
---
