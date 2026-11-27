---
anonymous_access: true
api_key_in: []
api_specs:
- filename: comparecallanswering-com-enquiry-api-openapi.yml
  format: yaml
  label: Compare Call Answering Enquiry API
  slug: comparecallanswering-com-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparecallanswering-com/openapi/comparecallanswering-com-enquiry-api-openapi.yml
- filename: comparecallanswering-com-guide-api-openapi.yml
  format: yaml
  label: Compare Call Answering Guide API
  slug: comparecallanswering-com-guide-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparecallanswering-com/openapi/comparecallanswering-com-guide-api-openapi.yml
- filename: comparecallanswering-com-mcp-api-openapi.yml
  format: yaml
  label: Compare Call Answering MCP API
  slug: comparecallanswering-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/comparecallanswering-com/openapi/comparecallanswering-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Compare Call Answering Authentication
name_suffix: Authentication
oauth_flows: []
overview: Compare Call Answering secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Compare Call Answering
provider_slug: comparecallanswering-com
scheme_count: 2
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  key_prefix: emk_
  name: accessKey
  required: false
  scheme: bearer
  sources:
  - openapi/comparecallanswering-com-openapi.yml
  type: http
- description: MCP server card states "auth":"none" for the Streamable HTTP endpoint at https://comparecallanswering.com/mcp.
  name: none
  sources:
  - https://comparecallanswering.com/mcp
  type: none
slug: comparecallanswering-com-authentication
source_filename: comparecallanswering-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://comparecallanswering.com/mcp\ndocs: https://comparecallanswering.com/mcp\nsummary:\n  types:\n  - http\n  optional: true\n  note: Authentication is optional. The OpenAPI declares a bearer access key (emk_...) that raises the free-tier ceiling\n    to a named budget; the MCP server card (GET https://comparecallanswering.com/mcp, HTTP 200) declares \"auth\":\"none\"\n    for the MCP transport. No key issuance page is published; the 429 descriptions reference docs/MCP.md, which returned\n    HTTP 404 at https://comparecallanswering.com/docs/MCP.md.\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  key_prefix: emk_\n  required: false\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'\n  sources:\n  - openapi/comparecallanswering-com-openapi.yml\n- name: none\n  type: none\n  description: MCP server card states \"auth\":\"none\" for\
  \ the Streamable HTTP endpoint at https://comparecallanswering.com/mcp.\n  sources:\n  - https://comparecallanswering.com/mcp\n"
source_yaml_url: https://artifacts.apis.io/comparecallanswering-com/authentication/comparecallanswering-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Call Answering
- AI Voice Agents
- Answering Services
- Comparison
- Telephony
- Compliance
- MCP
---
