---
api_key_in:
- header
api_specs:
- filename: monetizenow-openapi.json
  format: json
  label: MonetizeNow API
  slug: monetizenow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/monetizenow/refs/heads/main/openapi/monetizenow-openapi.json
auth_types:
- apiKey
- oauth2
description: MonetizeNow has two distinct authentication surfaces. The documented REST API uses a single tenant-generated API key in an x-api-key header, with no scopes and no test/live key separation. The undocumented but live MCP server at mcp.monetizeplatform.com uses OAuth 2.x bearer tokens with dynamic client registration and PKCE S256, discovered from its own RFC 8414 / RFC 9728 metadata.
kind: authentication
layout: security
method: searched
name: Monetizenow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: MonetizeNow secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: MonetizeNow
provider_slug: monetizenow
scheme_count: 2
schemes:
- applies_to: https://api.monetizeplatform.com (all REST operations)
  description: The preferred (and documented) authentication method is a tenant-generated API key sent in the x-api-key request header. Keys are created in the MonetizeNow tenant under Settings -> API Keys ("New Api Key"), named, and displayed only once at creation. A single key authenticates against all MonetizeNow REST APIs.
  in: header
  key_prefix: not published
  name: apiKey
  parameter_name: x-api-key
  provisioning: MonetizeNow tenant UI (Settings -> API Keys)
  rotation_policy: not published
  scoped: false
  sources:
  - https://docs.monetizenow.io/reference/getting-started-with-your-api
  - https://docs.monetizenow.io/docs/api-keys
  type: apiKey
- applies_to: https://mcp.monetizeplatform.com/mcp
  description: 'OAuth 2.x bearer, discovered live. Unauthenticated requests return HTTP 401 with WWW-Authenticate: Bearer realm="mcp". Dynamic client registration is open at /oauth/register; PKCE S256 required; token endpoint auth method "none" (public clients).'
  detail: scopes/monetizenow-scopes.yml
  discovery:
  - spec: RFC 8414
    status: 200
    url: https://mcp.monetizeplatform.com/.well-known/oauth-authorization-server
  - spec: RFC 9728
    status: 200
    url: https://mcp.monetizeplatform.com/.well-known/oauth-protected-resource
  flows:
  - authorizationUrl: https://mcp.monetizeplatform.com/oauth/authorize
    flow: authorizationCode
    refreshSupported: true
    scopes: {}
    tokenUrl: https://mcp.monetizeplatform.com/oauth/token
  name: mcpOAuth
  scoped: false
  sources:
  - https://mcp.monetizeplatform.com/.well-known/oauth-authorization-server
  type: oauth2
slug: monetizenow-authentication
source_filename: monetizenow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.monetizenow.io/reference/getting-started-with-your-api\ndocs: https://docs.monetizenow.io/docs/api-keys\nbase_url: https://api.monetizeplatform.com\ndescription: >-\n  MonetizeNow has two distinct authentication surfaces. The documented REST API\n  uses a single tenant-generated API key in an x-api-key header, with no scopes\n  and no test/live key separation. The undocumented but live MCP server at\n  mcp.monetizeplatform.com uses OAuth 2.x bearer tokens with dynamic client\n  registration and PKCE S256, discovered from its own RFC 8414 / RFC 9728\n  metadata.\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  applies_to: https://api.monetizeplatform.com (all REST operations)\n  description: >-\n    The preferred (and documented) authentication method is a tenant-generated\n\
  \    API key sent in the x-api-key request header. Keys are created in the\n    MonetizeNow tenant under Settings -> API Keys (\"New Api Key\"), named, and\n    displayed only once at creation. A single key authenticates against all\n    MonetizeNow REST APIs.\n  provisioning: MonetizeNow tenant UI (Settings -> API Keys)\n  scoped: false\n  key_prefix: not published\n  rotation_policy: not published\n  sources:\n  - https://docs.monetizenow.io/reference/getting-started-with-your-api\n  - https://docs.monetizenow.io/docs/api-keys\n- name: mcpOAuth\n  type: oauth2\n  applies_to: https://mcp.monetizeplatform.com/mcp\n  description: >-\n    OAuth 2.x bearer, discovered live. Unauthenticated requests return HTTP 401\n    with WWW-Authenticate: Bearer realm=\"mcp\". Dynamic client registration is\n    open at /oauth/register; PKCE S256 required; token endpoint auth method\n    \"none\" (public clients).\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://mcp.monetizeplatform.com/oauth/authorize\n\
  \    tokenUrl: https://mcp.monetizeplatform.com/oauth/token\n    refreshSupported: true\n    scopes: {}\n  discovery:\n  - {spec: 'RFC 8414', url: 'https://mcp.monetizeplatform.com/.well-known/oauth-authorization-server', status: 200}\n  - {spec: 'RFC 9728', url: 'https://mcp.monetizeplatform.com/.well-known/oauth-protected-resource', status: 200}\n  scoped: false\n  detail: scopes/monetizenow-scopes.yml\n  sources:\n  - https://mcp.monetizeplatform.com/.well-known/oauth-authorization-server\nnotes:\n- >-\n  The REST key is tenant-wide and unscoped: one key grants access to every\n  MonetizeNow REST API in the tenant. No read-only key type, no per-resource\n  permission, and no key prefix convention are published.\n- >-\n  No test-vs-live key separation is documented; see sandbox/monetizenow-sandbox.yml.\n- >-\n  The application console (app.monetizeplatform.com) uses a separate interactive\n  login and, per the Information Security Policy, SSO/SAML with MFA for workforce\n  access. That\
  \ is human sign-in, not API authentication.\n- >-\n  The OAuth authorization server publishes no scope vocabulary\n  (scopes_supported: []), so an MCP client cannot request narrowed access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/monetizenow/refs/heads/main/authentication/monetizenow-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Monetization
- Billing
- Subscription
- Usage-Based Pricing
- Quote-to-Cash
- CPQ
- Payments
- Invoicing
- Revenue
- Software-as-a-Service
- Fintech
---
