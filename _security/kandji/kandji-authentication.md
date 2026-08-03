---
api_key_in:
- header
api_specs:
- filename: kandji-endpoint-management-openapi.json
  format: json
  label: Iru Endpoint Management API
  slug: iru-endpoint-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-endpoint-management-openapi.json
- filename: kandji-upload-to-s3-openapi.json
  format: json
  label: Iru Library Item Upload API
  slug: iru-library-item-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-upload-to-s3-openapi.json
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Kandji Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iru secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Iru
provider_slug: kandji
scheme_count: 3
schemes:
- applied: globally via the spec root security[]; every one of the 121 operations inherits it
  bearerFormat: JWT
  header: Authorization
  name: BearerAuth
  note: 'The spec declares bearerFormat: JWT, but the docs describe the credential only as a "tenant-level bearer token"; the token''s internal format is not documented and should not be parsed by clients.'
  scheme: bearer
  sources:
  - openapi/kandji-endpoint-management-openapi.json
  surface: rest
  type: http
  value_format: Bearer <token>
- in: header
  name: MCP X-API-Key
  parameter: X-API-Key
  sources:
  - https://docs.iru.com/en/endpoint/integrations/ai-assistants/iru-mcp
  surface: mcp
  type: apiKey
  value_format: sk_live:<key>
- in: header
  name: MCP X-MCP-Profile
  parameter: X-MCP-Profile
  role: selects the MCP profile issued with the token
  sources:
  - https://docs.iru.com/en/endpoint/integrations/ai-assistants/iru-mcp
  surface: mcp
  type: apiKey
slug: kandji-authentication
source_filename: kandji-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: >-\n  openapi/kandji-endpoint-management-openapi.json (derived) upgraded with\n  https://docs.iru.com/en/endpoint/api/iru-api-overview and\n  https://docs.iru.com/en/endpoint/integrations/ai-assistants/iru-mcp (searched)\ndocs: https://docs.iru.com/en/endpoint/api/iru-api-overview\nsummary:\n  types:\n  - http\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    Two distinct credentials, both minted from the same object. A single API token created in\n    Access is used as an HTTP bearer token for REST, and — only if \"Enable MCP\" was switched on\n    before Create — the same token issuance also produces an MCP configuration whose X-API-Key\n    header value carries an `sk_live:` prefix. No OAuth 2.0, no OpenID Connect, no mutual TLS.\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  surface: rest\n  header: Authorization\n  value_format: 'Bearer <token>'\n  applied:\
  \ globally via the spec root security[]; every one of the 121 operations inherits it\n  sources:\n  - openapi/kandji-endpoint-management-openapi.json\n  note: >-\n    The spec declares bearerFormat: JWT, but the docs describe the credential only as a\n    \"tenant-level bearer token\"; the token's internal format is not documented and should not be\n    parsed by clients.\n- name: MCP X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  value_format: 'sk_live:<key>'\n  surface: mcp\n  sources:\n  - https://docs.iru.com/en/endpoint/integrations/ai-assistants/iru-mcp\n- name: MCP X-MCP-Profile\n  type: apiKey\n  in: header\n  parameter: X-MCP-Profile\n  surface: mcp\n  role: selects the MCP profile issued with the token\n  sources:\n  - https://docs.iru.com/en/endpoint/integrations/ai-assistants/iru-mcp\ntoken_lifecycle:\n  issuance: Web App > Account Menu > Access > API tokens > Add Token (name + description required)\n  scope: tenant\n  one_time_display: true\n  one_time_display_note:\
  \ >-\n    The token value and the MCP configuration JSON are shown once, on the creation success screen.\n    If lost, the token must be revoked and re-created.\n  rotation_policy_documented: false\n  expiry_documented: false\n  revocation: 'Access > API tokens; revoking a token kills both its REST and its MCP access.'\n  audit: >-\n    Token created / updated / deleted events appear in the tenant-wide Unified Activity timeline and\n    on each token's Activity tab; the API also exposes /api/v1/audit/events (listAuditEvents).\nauthorization:\n  model: per-endpoint permission grid\n  granularity: individual endpoint, groupable by category (e.g. \"Blueprints Management\")\n  configurable: at creation (\"Configure\") or later (\"Edit\")\n  default: a token can be created with no permissions and configured later\n  scopes: null\n  scopes_note: >-\n    This is NOT an OAuth scope model — there is no scope string, no consent screen and no\n    authorization server, so no scopes/ artifact is emitted.\
  \ Authorization is an operator-selected\n    allowlist of API endpoints attached to the token.\n  applies_to_mcp: true\nregions:\n  us: https://{subdomain}.api.kandji.io\n  eu: https://{subdomain}.api.eu.kandji.io\n  note: >-\n    A token is bound to its tenant's regional hostname, shown as \"Your organization's API URL\" on\n    the Access > API tokens page.\nfailure_modes:\n  '401': Missing, malformed, revoked or wrong-tenant token (declared on 113 of 121 operations).\n  '403': Not declared anywhere in the spec — how an insufficient-permission denial surfaces is undocumented.\nsee_also:\n  conventions: conventions/kandji-conventions.yml\n  errors: errors/kandji-problem-types.yml\n  mcp: mcp/kandji-mcp.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/authentication/kandji-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Company
- device-management
- mobile-device-management
- apple-management
- endpoint-security
- endpoint-detection-response
- vulnerability-management
- compliance-automation
- workforce-identity
- it-operations
- mcp
- agent-native
---
