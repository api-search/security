---
anonymous_access: false
api_key_in: []
api_specs:
- filename: difcvsadgm-com-enquiry-api-openapi.yml
  format: yaml
  label: DIFC vs ADGM Enquiry API
  slug: difcvsadgm-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difcvsadgm-com/openapi/difcvsadgm-com-enquiry-api-openapi.yml
- filename: difcvsadgm-com-guide-api-openapi.yml
  format: yaml
  label: DIFC vs ADGM Guide API
  slug: difcvsadgm-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difcvsadgm-com/openapi/difcvsadgm-com-guide-api-openapi.yml
- filename: difcvsadgm-com-mcp-api-openapi.yml
  format: yaml
  label: DIFC vs ADGM MCP API
  slug: difcvsadgm-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/difcvsadgm-com/openapi/difcvsadgm-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Difcvsadgm Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DIFC vs ADGM secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DIFC vs ADGM
provider_slug: difcvsadgm-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  optional: true
  scheme: bearer
  sources:
  - openapi/difcvsadgm-com-openapi.yml
  - https://difcvsadgm.com/mcp
  type: http
slug: difcvsadgm-com-authentication
source_filename: difcvsadgm-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource: https://difcvsadgm.com/openapi.json\ndocs: https://difcvsadgm.com/mcp\nsummary:\n  types:\n  - http\n  anonymous_access: true\n  note: 'Every operation declares security [{}, {accessKey: []}] -- anonymous calls are allowed on a free tier; a bearer access key (emk_...) attaches a named budget. The provider''s MCP card (GET https://difcvsadgm.com/mcp, HTTP 200) states \"auth\": \"none\" for the MCP endpoint. No page documents how to obtain a key.'\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  key_prefix: emk_\n  optional: true\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/difcvsadgm-com-openapi.yml\n  - https://difcvsadgm.com/mcp\n"
source_yaml_url: https://artifacts.apis.io/difcvsadgm-com/authentication/difcvsadgm-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Company Formation
- Free Zones
- United Arab Emirates
- Financial Regulation
- Licensing
- MCP
---
