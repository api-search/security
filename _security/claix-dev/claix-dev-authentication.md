---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: claix-dev-openapi.yml
  format: yaml
  label: Claix Document Intelligence API
  slug: claix-document-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/claix-dev/refs/heads/main/openapi/claix-dev-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Claix Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Claix secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Claix
provider_slug: claix-dev
scheme_count: 2
schemes:
- description: Secret server API key. Takes priority over Authorization when both headers are sent. (Spec text, Spanish - "API key secreta de servidor. Tiene prioridad sobre Authorization si se envían ambos headers.")
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  recommended: true
  sources:
  - openapi/claix-dev-openapi.yml
  - https://www.claix.dev/documentation/excel-to-json
  surfaces:
  - rest
  - mcp
  - a2a
  type: apiKey
- description: Alternative way to send the same API key, as a Bearer token in Authorization. (Spec text - "Forma alternativa de enviar la API key como Bearer token.")
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/claix-dev-openapi.yml
  - https://www.claix.dev/documentation/a2a
  surfaces:
  - rest
  - a2a
  type: http
slug: claix-dev-authentication
source_filename: claix-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\nsource: openapi/claix-dev-openapi.yml\ndocs: https://www.claix.dev/documentation/excel-to-json\ndocs_also:\n  - https://www.claix.dev/documentation/sdks\n  - https://www.claix.dev/documentation/mcp\n  - https://www.claix.dev/documentation/a2a\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  one_credential_three_surfaces: >-\n    A single secret API key, issued in the dashboard (Workspace > API Keys), authenticates the\n    REST routes, the MCP server (x-api-key header, or api_key tool argument) and the A2A JSON-RPC\n    endpoint (x-api-key or Bearer). The agent card, openapi.yaml, llms.txt and MCP tools/list are\n    public and need no key.\n  key_format: >-\n    Not published in the spec. The SDK docs show the placeholder \"ck_...\" (CLAIX_API_KEY=ck_...)\n    while the MCP tool schema example reads \"claix_sk_abc123...\"; treated as unknown rather than\n    asserted.\n  precedence: x-api-key takes priority\
  \ when both headers are sent (spec + docs).\n  scope: >-\n    Key -> one workspace/account. Every schema, persisted document and knowledge space is owned by\n    the key's account; ids that belong to another account return 404, not 403.\n  validation: >-\n    Before any file is processed the server checks that the key exists and is active and that the\n    account is not suspended; failure is 401 with the {error, detalle} envelope and nothing is\n    billed.\n  no_oauth: No OAuth 2.0 / OIDC; /.well-known/oauth-authorization-server, oauth-protected-resource and openid-configuration all 404 (well-known/claix-dev-well-known.yml).\n  client_side: >-\n    The docs forbid calling the API from an end-user browser (\"requires a secret API key ...\n    handle with the same care as a database password\"); the embeddable widget exists precisely so\n    the key stays server-side (components/claix-dev-components.yml).\n  env_var: CLAIX_API_KEY (Python SDK)\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n\
  \  in: header\n  parameter: x-api-key\n  description: Secret server API key. Takes priority over Authorization when both headers are sent. (Spec text, Spanish - \"API key secreta de servidor. Tiene prioridad sobre Authorization si se envían ambos headers.\")\n  recommended: true\n  surfaces: [rest, mcp, a2a]\n  sources:\n  - openapi/claix-dev-openapi.yml\n  - https://www.claix.dev/documentation/excel-to-json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Alternative way to send the same API key, as a Bearer token in Authorization. (Spec text - \"Forma alternativa de enviar la API key como Bearer token.\")\n  surfaces: [rest, a2a]\n  sources:\n  - openapi/claix-dev-openapi.yml\n  - https://www.claix.dev/documentation/a2a\nmcp_specific:\n  header: x-api-key\n  tool_argument_fallback: api_key (string, minLength 8) on every tool, for clients that cannot set headers\n  smithery: registry config field APIKEY mapped to the x-api-key header (x-to)\na2a_specific:\n  error_on_missing_key:\
  \ 'HTTP 401, JSON-RPC {code: -32001, message: \"Unauthorized: send x-api-key or Authorization: Bearer.\"}'\n  observed: '2026-09-19 anonymous POST https://www.claix.dev/a2a -> 401 with exactly that body'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/claix-dev/refs/heads/main/authentication/claix-dev-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Document Processing
- Data Extraction
- Document Intelligence
- PDF
- Excel
- OCR
- Structured Data
- AI Agents
- MCP
- A2A
- Spain
- Company
---
