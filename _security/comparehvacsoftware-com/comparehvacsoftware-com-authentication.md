---
anonymous_access: true
api_key_in: []
api_specs:
- filename: comparehvacsoftware-com-enquiry-api-openapi.yml
  format: yaml
  label: Compare HVAC Software Enquiry API
  slug: comparehvacsoftware-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparehvacsoftware-com/openapi/comparehvacsoftware-com-enquiry-api-openapi.yml
- filename: comparehvacsoftware-com-guide-api-openapi.yml
  format: yaml
  label: Compare HVAC Software Guide API
  slug: comparehvacsoftware-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparehvacsoftware-com/openapi/comparehvacsoftware-com-guide-api-openapi.yml
- filename: comparehvacsoftware-com-mcp-api-openapi.yml
  format: yaml
  label: Compare HVAC Software MCP API
  slug: comparehvacsoftware-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparehvacsoftware-com/openapi/comparehvacsoftware-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Compare HVAC Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compare HVAC Software secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Compare HVAC Software
provider_slug: comparehvacsoftware-com
scheme_count: 2
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  optional: true
  scheme: bearer
  sources:
  - openapi/comparehvacsoftware-com-openapi.yml
  type: http
- description: MCP endpoint advertised with "auth":"none" (stateless, JSON responses).
  name: none
  sources:
  - https://comparehvacsoftware.com/mcp
  type: none
slug: comparehvacsoftware-com-authentication
source_filename: comparehvacsoftware-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comparehvacsoftware.com/mcp\ndocs: https://comparehvacsoftware.com/mcp\nsummary:\n  types:\n  - http\n  anonymous_access: true\n  note: The MCP card at https://comparehvacsoftware.com/mcp declares \"auth\":\"none\" for the streamable-http server; the OpenAPI declares an optional bearer access key (emk_...) that raises the free-tier ceiling. No OAuth, no scopes. The access-key issuance process is not documented on any page found (the 429 description points to docs/MCP.md, which returned 404 at https://comparehvacsoftware.com/docs/MCP.md on 2026-11-04).\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  optional: true\n  key_prefix: emk_\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/comparehvacsoftware-com-openapi.yml\n- name: none\n  type: none\n  description: MCP endpoint advertised with \"auth\"\
  :\"none\" (stateless, JSON responses).\n  sources:\n  - https://comparehvacsoftware.com/mcp\n"
source_yaml_url: https://artifacts.apis.io/comparehvacsoftware-com/authentication/comparehvacsoftware-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- HVAC
- Field Service Management
- Software Comparison
- EPA Section 608
- Compliance
- MCP
---
