---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agree-com-agreements-api-openapi.yml
  format: yaml
  label: Agree.com Agreements API
  slug: agree-com-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-agreements-api-openapi.yml
- filename: agree-com-contacts-api-openapi.yml
  format: yaml
  label: Agree.com Contacts API
  slug: agree-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-contacts-api-openapi.yml
- filename: agree-com-customers-api-openapi.yml
  format: yaml
  label: Agree.com Customers API
  slug: agree-com-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-customers-api-openapi.yml
- filename: agree-com-invoices-api-openapi.yml
  format: yaml
  label: Agree.com Invoices API
  slug: agree-com-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-invoices-api-openapi.yml
- filename: agree-com-reports-api-openapi.yml
  format: yaml
  label: Agree.com Reports API
  slug: agree-com-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-reports-api-openapi.yml
- filename: agree-com-webhooks-api-openapi.yml
  format: yaml
  label: Agree.com Webhooks API
  slug: agree-com-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/openapi/agree-com-webhooks-api-openapi.yml
auth_types:
- http
- oauth2
description: 'Agree.com runs two independent authentication models for two different surfaces. The REST API is protected by a long-lived bearer API key minted in the dashboard. The hosted MCP server is protected by a full OAuth 2.1 authorization server with PKCE and dynamic client registration. Neither is usable against the other: the OAuth server advertises exactly one scope, "mcp", and the REST spec declares only the bearer scheme.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Agree Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agree.com secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Agree.com
provider_slug: agree-com
scheme_count: 2
schemes:
- applied: 'Declared in components.securitySchemes and applied per-operation. All 56 operations carry security: [{bearer: []}]. The top-level security[] array is empty, so there is no document-wide default - the requirement is stated on every operation instead.'
  credential:
    kind: api-key
    prefix: null
    prefix_note: The documentation does not publish a key prefix or any test/live key distinction.
    provisioning: Generated in the Agree dashboard under Settings > API Keys.
    rotation: '"If compromised, regenerate it immediately in your dashboard." Rotation is manual and dashboard-only; no rotation endpoint exists in the API.'
    scoping: None. The documentation states plainly - "Keep this key secure - it provides full access to your organization's data." The key is organization-wide and unscoped; there is no read-only key, no per-resource restriction, and no documented expiry.
    transport: 'Authorization: Bearer <API_KEY>'
  description: API key authentication via Bearer token
  name: bearer
  scheme: bearer
  sources:
  - openapi/agree-com-api-openapi.json
  - https://secure.agree.com/documentation
  surface: REST API (https://secure.agree.com/api/v1)
  type: http
- bearer_methods_supported:
  - header
  client_authentication:
  - none
  - client_secret_post
  - client_secret_basic
  description: OAuth 2.1 authorization code flow protecting the hosted MCP endpoint. Not declared in the OpenAPI - it was found by probing RFC 8414 authorization server metadata and RFC 9728 protected resource metadata, both of which are served anonymously.
  dynamic_client_registration: true
  endpoints:
    issuer: https://secure.agree.com
    registration_endpoint: https://secure.agree.com/oauth/register
    revocation_endpoint: https://secure.agree.com/oauth/revoke
  flows:
    authorization_code:
      authorization_url: https://secure.agree.com/oauth/authorize
      pkce: S256
      pkce_required: true
      refresh_supported: true
      scopes:
        mcp: The single scope the authorization server advertises. Its grants are not documented; see scopes/agree-com-scopes.yml.
      token_url: https://secure.agree.com/oauth/token
  name: oauth2-mcp
  sources:
  - https://secure.agree.com/.well-known/oauth-authorization-server
  - https://secure.agree.com/.well-known/oauth-protected-resource
  surface: MCP server (https://secure.agree.com/mcp)
  type: oauth2
slug: agree-com-authentication
source_filename: agree-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  https://secure.agree.com/documentation (Introduction > Authentication) +\n  openapi/agree-com-api-openapi.json (components.securitySchemes) +\n  https://secure.agree.com/.well-known/oauth-authorization-server\ndocs: https://secure.agree.com/documentation#section/Introduction/Authentication\nname: Agree.com Authentication\ndescription: >-\n  Agree.com runs two independent authentication models for two different surfaces. The REST\n  API is protected by a long-lived bearer API key minted in the dashboard. The hosted MCP\n  server is protected by a full OAuth 2.1 authorization server with PKCE and dynamic client\n  registration. Neither is usable against the other: the OAuth server advertises exactly one\n  scope, \"mcp\", and the REST spec declares only the bearer scheme.\nsummary:\n  types:\n  - http\n  - oauth2\n  surfaces: 2\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  surface: REST API (https://secure.agree.com/api/v1)\n\
  \  description: API key authentication via Bearer token\n  applied: >-\n    Declared in components.securitySchemes and applied per-operation. All 56 operations carry\n    security: [{bearer: []}]. The top-level security[] array is empty, so there is no\n    document-wide default - the requirement is stated on every operation instead.\n  credential:\n    kind: api-key\n    provisioning: Generated in the Agree dashboard under Settings > API Keys.\n    transport: 'Authorization: Bearer <API_KEY>'\n    prefix: null\n    prefix_note: The documentation does not publish a key prefix or any test/live key distinction.\n    scoping: >-\n      None. The documentation states plainly - \"Keep this key secure - it provides full access\n      to your organization's data.\" The key is organization-wide and unscoped; there is no\n      read-only key, no per-resource restriction, and no documented expiry.\n    rotation: >-\n      \"If compromised, regenerate it immediately in your dashboard.\" Rotation\
  \ is manual and\n      dashboard-only; no rotation endpoint exists in the API.\n  sources:\n  - openapi/agree-com-api-openapi.json\n  - https://secure.agree.com/documentation\n- name: oauth2-mcp\n  type: oauth2\n  surface: MCP server (https://secure.agree.com/mcp)\n  description: >-\n    OAuth 2.1 authorization code flow protecting the hosted MCP endpoint. Not declared in the\n    OpenAPI - it was found by probing RFC 8414 authorization server metadata and RFC 9728\n    protected resource metadata, both of which are served anonymously.\n  flows:\n    authorization_code:\n      authorization_url: https://secure.agree.com/oauth/authorize\n      token_url: https://secure.agree.com/oauth/token\n      refresh_supported: true\n      pkce: S256\n      pkce_required: true\n      scopes:\n        mcp: >-\n          The single scope the authorization server advertises. Its grants are not documented;\n          see scopes/agree-com-scopes.yml.\n  endpoints:\n    issuer: https://secure.agree.com\n\
  \    registration_endpoint: https://secure.agree.com/oauth/register\n    revocation_endpoint: https://secure.agree.com/oauth/revoke\n  client_authentication:\n  - none\n  - client_secret_post\n  - client_secret_basic\n  dynamic_client_registration: true\n  bearer_methods_supported:\n  - header\n  sources:\n  - https://secure.agree.com/.well-known/oauth-authorization-server\n  - https://secure.agree.com/.well-known/oauth-protected-resource\nwebhook_verification:\n  mechanism: HMAC-SHA256\n  header: X-Webhook-Signature\n  timestamp_header: X-Webhook-Timestamp\n  encoding: hex, lowercase\n  secret: >-\n    Per-endpoint signing secret (whsec_ prefix) returned exactly once, in the response to\n    POST /api/v1/webhooks. It is not retrievable afterwards.\n  computation: HMAC-SHA256 over the raw request body, keyed by the endpoint secret.\n  comparison: >-\n    Constant-time. The documentation ships working Node.js (crypto.timingSafeEqual) and\n    Python (hmac.compare_digest) verification examples.\n\
  \  replay_protection: >-\n    PARTIAL. A timestamp header is sent but the documented verification procedure does not\n    include it in the signed payload and states no tolerance window, so the published\n    recipe does not by itself defeat replay.\n  source: https://secure.agree.com/documentation#tag/Webhooks\nfindings:\n- >-\n  The REST API has no OAuth, no scopes, and no key scoping. A single compromised key is full\n  organization access to contracts, invoices, contacts and revenue reporting.\n- >-\n  The MCP surface is materially better authenticated than the REST surface it fronts, which\n  is an unusual inversion - most providers in the catalog bolt a weaker key model onto MCP,\n  not a stronger one.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agree-com/refs/heads/main/authentication/agree-com-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Agreements
- Electronic Signature
- Contract Management
- Invoicing
- Billing
- Payments
- Accounts Receivable
- Fintech
- Financial-Services
- Webhook
- MCP
- agent-native
---
