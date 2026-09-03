---
api_key_in:
- header
api_specs:
- filename: vergesense-api-openapi.json
  format: json
  label: VergeSense API
  slug: vergesense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/openapi/vergesense-api-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Vergesense Authentication
name_suffix: Authentication
oauth_flows: []
overview: VergeSense secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VergeSense
provider_slug: vergesense
scheme_count: 2
schemes:
- applies_to: every operation in openapi/vergesense-api-openapi.json (36 operations)
  failure_reason: missing vs-api-key header or invalid API token
  failure_status: 403
  in: header
  name: sec0
  parameter: vs-api-key
  required: true
  sources:
  - openapi/vergesense-api-openapi.json
  - https://vergesense.readme.io/reference/reference-getting-started
  surface: rest
  transport: https only — requests to http:// are rejected
  type: apiKey
- authorization_endpoint: https://vergesense.auth0.com/authorize
  authorization_servers:
  - https://vergesense.auth0.com/
  bearer_methods_supported:
  - header
  discovery: https://mcp.vergesense.com/.well-known/oauth-protected-resource/mcp
  dynamic_client_registration: true
  method: probed
  name: mcp-oauth
  note: 'An anonymous POST of tools/list to https://mcp.vergesense.com/mcp returns HTTP 401 with WWW-Authenticate: Bearer resource_metadata="https://mcp.vergesense.com/.well-known/oauth-protected-resource/mcp". The live tool schemas are therefore auth-gated and were not read.'
  probed: '2026-09-02'
  registration_endpoint: https://vergesense.auth0.com/oidc/register
  resource: https://mcp.vergesense.com/mcp
  rfc: RFC 9728 (OAuth 2.0 Protected Resource Metadata)
  surface: mcp
  token_endpoint: https://vergesense.auth0.com/oauth/token
  type: oauth2
slug: vergesense-authentication
source_filename: vergesense-authentication.yml
source_heading: Authentication Profile
source_url: https://vergesense.readme.io/reference/reference-getting-started
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://vergesense.readme.io/reference/reference-getting-started\nsources:\n- https://vergesense.readme.io/reference/reference-getting-started\n- https://vergesense.readme.io/reference/events\n- openapi/vergesense-api-openapi.json\n- https://mcp.vergesense.com/.well-known/oauth-protected-resource/mcp\n- https://vergesense.auth0.com/.well-known/openid-configuration\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  note: >-\n    Two distinct authentication surfaces. The REST/Analytics API at api.vergesense.com is\n    API-key only (single header, no OAuth, no scopes). The remote MCP server at\n    mcp.vergesense.com is OAuth 2.0 bearer, delegated to the VergeSense Auth0 tenant and\n    advertised per RFC 9728.\n\nschemes:\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: vs-api-key\n  surface: rest\n  required: true\n  applies_to: every operation in openapi/vergesense-api-openapi.json (36 operations)\n\
  \  transport: https only — requests to http:// are rejected\n  failure_status: 403\n  failure_reason: missing vs-api-key header or invalid API token\n  sources:\n  - openapi/vergesense-api-openapi.json\n  - https://vergesense.readme.io/reference/reference-getting-started\n\n- name: mcp-oauth\n  type: oauth2\n  surface: mcp\n  resource: https://mcp.vergesense.com/mcp\n  authorization_servers:\n  - https://vergesense.auth0.com/\n  bearer_methods_supported:\n  - header\n  discovery: https://mcp.vergesense.com/.well-known/oauth-protected-resource/mcp\n  rfc: RFC 9728 (OAuth 2.0 Protected Resource Metadata)\n  authorization_endpoint: https://vergesense.auth0.com/authorize\n  token_endpoint: https://vergesense.auth0.com/oauth/token\n  registration_endpoint: https://vergesense.auth0.com/oidc/register\n  dynamic_client_registration: true\n  method: probed\n  probed: '2026-09-02'\n  note: >-\n    An anonymous POST of tools/list to https://mcp.vergesense.com/mcp returns HTTP 401 with\n    WWW-Authenticate:\
  \ Bearer resource_metadata=\"https://mcp.vergesense.com/.well-known/oauth-protected-resource/mcp\".\n    The live tool schemas are therefore auth-gated and were not read.\n\nkey_management:\n  issuance: >-\n    Not self-serve. The docs instruct prospective developers to contact support@vergesense.com to\n    request a VergeSense Developer account; keys are then generated inside the VergeSense Cloud app.\n  console_path: Settings > API Keys > Generate API Key\n  key_naming: an API Token Name is required at creation\n  scoping: >-\n    An API key is scoped to a selected set of buildings at creation, and the building selection can\n    be edited afterwards from Integrations > Details. This is the only authorization granularity the\n    REST API exposes — there are no OAuth scopes or per-endpoint permissions.\n  rotation: >-\n    Self-service rotation is published: Integrations > Details > Rotate generates a new API key.\n    The docs recommend periodic rotation and rotation on suspected compromise.\n\
  \  visibility: the key can be revealed in-app via Integrations > Details > Show\n  source: https://vergesense.readme.io/reference/reference-getting-started\n\nenvironments:\n- name: AWS (default)\n  base_url: https://api.vergesense.com\n- name: Azure\n  base_url: https://api.azure.vergesense.com\n  note: >-\n    Alternate deployment for Azure-hosted tenants. The published OpenAPI declares only the AWS host\n    in servers[]; the Azure host is documented in prose on the Getting Started page.\n\noutbound_webhook_authentication:\n  note: >-\n    Distinct from inbound API auth — this is how VergeSense authenticates ITSELF to a customer's\n    webhook receiver. Authentication is optional but recommended by the provider.\n  methods:\n  - technique: Basic access authentication\n    header: 'Basic: [base64(username:password)]'\n    configurable_in_ui: true\n  - technique: Bearer token\n    header: 'Bearer: [token]'\n    configurable_in_ui: true\n  - technique: Custom header\n    header: any key:value\
  \ pair\n    configurable_in_ui: true\n  - technique: OAuth 2.0\n    header: 'Bearer: [token] (after retrieving a token from the configured token URL)'\n    configurable_in_ui: false\n    reference: https://headwayapp.co/vergesense-changelog/bearer-token-authorization-webhook-support-137616\n  ip_allow_list:\n    available: true\n    self_serve: false\n    note: >-\n      VergeSense sends webhook requests from a known set of source IP addresses and will share the\n      list on request; it is not published in the documentation.\n  source: https://vergesense.readme.io/reference/events\n\ngaps:\n- No OAuth 2.0 or OIDC on the REST API — a single long-lived header key is the only credential.\n- No published scope or permission vocabulary for the REST API; authorization is building-level only.\n- No self-serve signup for API credentials; an email to support@vergesense.com gates access.\n- No documented key expiry or automatic rotation policy.\n- MCP tool schemas cannot be introspected anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vergesense/refs/heads/main/authentication/vergesense-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Occupancy Intelligence
- Workplace Analytics
- Corporate Real Estate
- PropTech
- IoT Sensors
- Building Data
- Space Utilization
- Facilities Management
- Smart Buildings
- Webhooks
- MCP
- JSON:API
---
