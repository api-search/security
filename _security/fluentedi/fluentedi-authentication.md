---
api_key_in: []
api_specs:
- filename: openapi.json
  format: json
  label: FluentEDI Tools API
  slug: fluentedi-tools-api
  spec_type: OpenAPI
  url: https://fluentedi.com/openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Fluentedi Authentication
name_suffix: Authentication
oauth_flows: []
overview: FluentEDI declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: FluentEDI
provider_slug: fluentedi
scheme_count: 0
schemes: []
slug: fluentedi-authentication
source_filename: fluentedi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: https://fluentedi.com/.well-known/ai\ndocs: https://fluentedi.com/llms.txt\nsummary: >-\n  FluentEDI publishes no authentication at all, and says so in four separate machine-readable places\n  rather than leaving it to be inferred. There is no account, no API key, no OAuth, no bearer token\n  and no signup on any surface - REST, batch or MCP.\nmodel: none\nschemes: []\nopenapi:\n  file: openapi/fluentedi-openapi.json\n  components_securitySchemes: []\n  security: absent\n  note: >-\n    The served OpenAPI 3.1 declares no securitySchemes and applies no security requirement to any of\n    its 99 operations. For most providers that would be a thin spec; here it is an accurate\n    description of the product, corroborated by the declarations below.\ndeclarations:\n- url: https://fluentedi.com/.well-known/ai\n  status: 200\n  says: 'authentication: {required: false, type: none}'\n- url: https://fluentedi.com/.well-known/ai-plugin.json\n\
  \  status: 200\n  says: 'auth: {type: none}'\n- url: https://fluentedi.com/.well-known/mcp.json\n  status: 200\n  says: 'authentication: {type: none}'\n- url: https://fluentedi.com/.well-known/mcp/server-card.json\n  status: 200\n  says: 'authentication: {type: none}'\n- url: https://fluentedi.com/v1/tools\n  status: 200\n  says: 'authentication: \"none\"'\nverification:\n  anonymous_rest_call:\n    url: https://fluentedi.com/v1/time/now?timezone=UTC\n    status: 200\n    note: Returned a tool result with no credential of any kind.\n  anonymous_mcp_tools_list:\n    url: https://fluentedi.com/mcp\n    status: 200\n    note: tools/list returned 19 tools with full inputSchemas and no OAuth challenge.\n  oauth_metadata:\n    '/.well-known/oauth-authorization-server': 404\n    '/.well-known/oauth-protected-resource': 404\n    '/.well-known/openid-configuration': 404\ncors:\n  access-control-allow-origin: '*'\n  access-control-allow-methods: GET, POST, HEAD, OPTIONS\n  access-control-allow-headers:\
  \ content-type, accept, mcp-protocol-version, mcp-session-id, authorization\n  note: Observed on a live response; browser-side agents can call the API directly.\nscopes: null\nscopes_note: No OAuth surface exists, so there is no scope model to document. scopes/ is intentionally absent.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fluentedi/refs/heads/main/authentication/fluentedi-authentication.yml
summary_line: 0 schemes
tags:
- EDI
- X12
- Retail EDI
- AI Agents
- MCP
- Developer Tools
- JSON
- Cryptography
- Data Validation
- Supply Chain
---
