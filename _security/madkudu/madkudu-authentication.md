---
api_key_in:
- header
- path
api_specs:
- filename: madkudu-madapi-openapi.yml
  format: yaml
  label: MadKudu API (MadAPI)
  slug: madkudu-api-madapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madkudu/refs/heads/main/openapi/madkudu-madapi-openapi.yml
- filename: madkudu-legacy-api-openapi.yml
  format: yaml
  label: MadKudu Legacy Scoring API
  slug: madkudu-legacy-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/madkudu/refs/heads/main/openapi/madkudu-legacy-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Madkudu Authentication
name_suffix: Authentication
oauth_flows: []
overview: MadKudu secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MadKudu
provider_slug: madkudu
scheme_count: 3
schemes:
- applies_to: MadKudu API (MadAPI)
  declared_in: openapi/madkudu-madapi-openapi.yml (components.securitySchemes.ApiKeyAuth)
  description: MadAPI authenticates with a raw API key sent in the x-api-key request header on every request. HTTPS is mandatory; calls over plain HTTP fail. Base URL https://madapi.madkudu.com (staging https://madapi.wisekudu.com). The docs spell the header `X-API-Key` and the published OpenAPI declares `x-api-key` — HTTP header names are case-insensitive, so both work.
  in: header
  name: ApiKeyAuth
  parameter_name: x-api-key
  security_applied: 'Global — `security: [{ApiKeyAuth: []}]` at the document root, so every MadAPI operation requires it.'
  type: apiKey
- applies_to: MadKudu Legacy Scoring API
  declared_in: openapi/madkudu-legacy-api-openapi.yml
  description: 'The legacy Scoring API uses HTTP Basic authentication with the API key as the username and an empty password — Base64 encode `YOUR_API_KEY:` (note the trailing colon) and send `Authorization: Basic <encoded>`. Base URL https://api.madkudu.com. The docs state this key is DIFFERENT from the MadAPI key.'
  name: LegacyBasicAuth
  scheme: basic
  type: http
- applies_to: MadKudu MCP server (MadMCP)
  description: 'The hosted MCP server takes the same MadAPI key as a URL PATH SEGMENT — https://mcp.madkudu.com/YOUR_API_KEY/mcp (or /sse). The credential therefore travels in the URL, where it is exposed to proxy logs, browser history, MCP client config files and any tool that records server URLs, and it cannot be rotated per-request. MadKudu''s own integration docs tell Dust and n8n users to set "no Bearer token" / "Authentication: None" because the key is already in the path.'
  in: path
  name: MCPPathKey
  parameter_name: YOUR_API_KEY
  ref: mcp/madkudu-mcp.yml
  type: apiKey
slug: madkudu-authentication
source_filename: madkudu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: https://developers.madkudu.com/api/authentication\nderived_from:\n- openapi/madkudu-madapi-openapi.yml\n- openapi/madkudu-legacy-api-openapi.yml\ndocs:\n- https://developers.madkudu.com/api/authentication\n- https://developers.madkudu.com/getting-started/quickstart\n- https://developers.madkudu.com/legacy-api/authentication\nsummary:\n  types: [apiKey, http]\n  api_key_in: [header, path]\n  http_schemes: [basic]\n  oauth2_flows: []\n  oidc: false\n  mtls: false\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  declared_in: openapi/madkudu-madapi-openapi.yml (components.securitySchemes.ApiKeyAuth)\n  security_applied: >-\n    Global — `security: [{ApiKeyAuth: []}]` at the document root, so every MadAPI operation\n    requires it.\n  description: >-\n    MadAPI authenticates with a raw API key sent in the x-api-key request header on every request.\n    HTTPS is mandatory; calls over plain\
  \ HTTP fail. Base URL https://madapi.madkudu.com\n    (staging https://madapi.wisekudu.com). The docs spell the header `X-API-Key` and the published\n    OpenAPI declares `x-api-key` — HTTP header names are case-insensitive, so both work.\n  applies_to: MadKudu API (MadAPI)\n- name: LegacyBasicAuth\n  type: http\n  scheme: basic\n  declared_in: openapi/madkudu-legacy-api-openapi.yml\n  description: >-\n    The legacy Scoring API uses HTTP Basic authentication with the API key as the username and an\n    empty password — Base64 encode `YOUR_API_KEY:` (note the trailing colon) and send\n    `Authorization: Basic <encoded>`. Base URL https://api.madkudu.com. The docs state this key is\n    DIFFERENT from the MadAPI key.\n  applies_to: MadKudu Legacy Scoring API\n- name: MCPPathKey\n  type: apiKey\n  in: path\n  parameter_name: YOUR_API_KEY\n  description: >-\n    The hosted MCP server takes the same MadAPI key as a URL PATH SEGMENT —\n    https://mcp.madkudu.com/YOUR_API_KEY/mcp (or /sse).\
  \ The credential therefore travels in the\n    URL, where it is exposed to proxy logs, browser history, MCP client config files and any tool\n    that records server URLs, and it cannot be rotated per-request. MadKudu's own integration docs\n    tell Dust and n8n users to set \"no Bearer token\" / \"Authentication: None\" because the key is\n    already in the path.\n  applies_to: MadKudu MCP server (MadMCP)\n  ref: mcp/madkudu-mcp.yml\nkey_management:\n  issuance: https://admin.madkudu.com > Personal Settings > My API Keys > Create API key\n  prerequisites:\n  - An active MadKudu account\n  - MadKudu Admin role\n  scoping: >-\n    Keys are PERSONAL — tied to the creating user and that user's permissions — and MadKudu\n    recommends creating a separate key per integration (named e.g. \"Cursor\", \"Zapier\", \"Claude\") so\n    usage can be attributed per key in Settings > API Usage.\n  rotation_policy: null\n  expiry: null\n  scopes: none — there is no OAuth scope or permission model\
  \ on the key itself; it inherits the\n    user's permissions.\n  warning: >-\n    \"Your API keys carry many privileges, so be sure to keep them secure! Do not share your secret\n    API keys in publicly accessible areas such as GitHub, client-side code, and so forth.\" —\n    published verbatim by MadKudu.\nnotes: >-\n  No OAuth 2.0, no OpenID Connect, no mutual TLS, and no /.well-known/ discovery document on any\n  host. Every surface is a single long-lived bearer-equivalent secret, and on the agent surface\n  that secret is in the URL.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/madkudu/refs/heads/main/authentication/madkudu-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Applicative Saas
- Sales Intelligence
- Lead Scoring
- Predictive Analytics
- Account Intelligence
- Data Enrichment
- MCP
- Agents
- Go-To-Market
---
