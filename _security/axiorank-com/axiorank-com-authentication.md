---
anonymous_access: false
api_key_in: []
api_specs:
- filename: axiorank-com-audit-api-openapi.yml
  format: yaml
  label: AxioRank Audit API
  slug: axiorank-com-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-audit-api-openapi.yml
- filename: axiorank-com-gateway-api-openapi.yml
  format: yaml
  label: AxioRank Gateway API
  slug: axiorank-com-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-gateway-api-openapi.yml
- filename: axiorank-com-health-api-openapi.yml
  format: yaml
  label: AxioRank Health API
  slug: axiorank-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-health-api-openapi.yml
- filename: axiorank-com-mcp-api-openapi.yml
  format: yaml
  label: AxioRank MCP API
  slug: axiorank-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-mcp-api-openapi.yml
- filename: axiorank-com-protocols-api-openapi.yml
  format: yaml
  label: AxioRank Protocols API
  slug: axiorank-com-protocols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-protocols-api-openapi.yml
- filename: axiorank-com-tools-log-api-openapi.yml
  format: yaml
  label: AxioRank Tools Log API
  slug: axiorank-com-tools-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/axiorank-com/openapi/axiorank-com-tools-log-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: AxioRank Authentication
name_suffix: Authentication
oauth_flows: []
overview: AxioRank secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AxioRank
provider_slug: axiorank-com
scheme_count: 1
schemes:
- description: 'An AxioRank API key (`axr_live_…` agent key or `axr_site_…` property key) or a short-lived token (`axr_tok_…`). Sent as `Authorization: Bearer <key>`. Scopes: `gateway:write`, `cards:verify`, `inbound:verify`, `logs:read`, `admin`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/axiorank-com-openapi.json
  type: http
slug: axiorank-com-authentication
source_filename: axiorank-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/axiorank-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An AxioRank API key (`axr_live_…` agent key or `axr_site_…` property key) or\n    a short-lived token (`axr_tok_…`). Sent as `Authorization: Bearer <key>`. Scopes: `gateway:write`,\n    `cards:verify`, `inbound:verify`, `logs:read`, `admin`.'\n  sources:\n  - openapi/axiorank-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/axiorank-com/authentication/axiorank-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Security
- Gateways
- Zero Trust
- Agents
---
