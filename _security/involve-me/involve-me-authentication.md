---
api_key_in: []
auth_types: []
description: How a machine authenticates to involve.me. There is no public REST API and therefore no API-key programme for one; the authenticated surfaces are the OAuth-protected MCP server, the outbound webhook (where involve.me is the client and the integrator supplies the credential), and the human-facing app with SSO on Enterprise. Each scheme below was observed or read on a provider page — none is inferred from a spec.
kind: authentication
layout: security
method: searched
name: Involve Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: involve.me declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: involve.me
provider_slug: involve-me
scheme_count: 5
schemes:
- applies_to: The Statamic CMS MCP server (marketing website content).
  bearer_methods_supported:
  - header
  dynamic_client_registration:
    client_id_metadata_document_supported: true
    registration_endpoint: https://www-cdn.involve.me/mcp/oauth/register
    supported: true
  evidence:
    http_status: 200
    url: https://www.involve.me/.well-known/oauth-authorization-server
  flows:
    authorization_code:
      authorization_url: https://www-cdn.involve.me/cp/mcp/oauth/authorize
      pkce: S256
      pkce_required: true
      refresh_supported: true
      token_url: https://www-cdn.involve.me/mcp/oauth/token
  id: mcp_oauth2
  method: probed
  revocation_endpoint: https://www-cdn.involve.me/mcp/oauth/revoke
  scopes: scopes/involve-me-scopes.yml
  surface: https://www-cdn.involve.me/mcp/statamic
  token_endpoint_auth_methods:
  - none
  type: oauth2
- alternate: basic
  applies_to: The same MCP server, as an alternative to the OAuth flow.
  detail: The unauthenticated 401 body states "Provide a Bearer token or Basic Auth credentials" and hints "Create an API token in the Statamic MCP dashboard" — i.e. a tenant-issued static token created inside the CMS control panel. No public documentation of that token's format, rotation or expiry exists.
  evidence:
    http_status: 401
    url: https://www-cdn.involve.me/mcp/statamic
    www_authenticate: Bearer realm="mcp"
  id: mcp_static_token
  method: probed
  scheme: bearer
  surface: https://www-cdn.involve.me/mcp/statamic
  type: http
- applies_to: involve.me POSTing submission data to the integrator's endpoint. involve.me is the CLIENT here; the integrator defines the credential.
  detail: The webhook configuration accepts one custom "Header Name" / "Header Value" pair, which involve.me sends on every delivery. This is the only authentication available on the webhook surface.
  direction: outbound
  evidence:
    http_status: 200
    url: https://help.involve.me/en/articles/2193514-receive-submission-data-with-webhooks-anywhere
  id: webhook_custom_header
  in: header
  method: searched
  name: user-defined
  signature_note: No HMAC signature, no signing secret and no timestamp header is documented. A receiver cannot cryptographically verify that a payload came from involve.me — a shared static header is the whole of the trust model.
  signature_verification: false
  surface: outbound webhook delivery
  type: apiKey
- applies_to: Human sign-in to the involve.me application.
  detail: Single sign-on is listed as an Enterprise-plan feature on the pricing page. The identity providers, protocol (SAML vs OIDC) and configuration are not publicly documented; involve.me publishes no /.well-known/openid-configuration (probed 404 on www. and app.).
  evidence:
    http_status: 200
    url: https://www.involve.me/pricing
  id: app_sso
  method: searched
  surface: https://app.involve.me/login
  type: openIdConnect
- applies_to: The product SPA's own backend.
  detail: app.involve.me/api/v1/* returns 302 to login for anonymous callers and the edge sets XSRF-TOKEN and lvapp_session cookies (Laravel). This is an internal, session-authenticated surface, not a published API — it is recorded for accuracy, not as an integration path.
  evidence:
    http_status: 302
    url: https://app.involve.me/api/v1/projects
  id: app_session
  method: probed
  scheme: cookie
  surface: https://app.involve.me
  type: http
slug: involve-me-authentication
source_filename: involve-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://www.involve.me/.well-known/oauth-authorization-server (200),\n  https://www.involve.me/.well-known/oauth-protected-resource (200),\n  https://help.involve.me/en/articles/2193514-receive-submission-data-with-webhooks-anywhere,\n  https://www.involve.me/pricing. Derived from no OpenAPI — involve.me publishes none.\ndescription: >-\n  How a machine authenticates to involve.me. There is no public REST API and\n  therefore no API-key programme for one; the authenticated surfaces are the\n  OAuth-protected MCP server, the outbound webhook (where involve.me is the client\n  and the integrator supplies the credential), and the human-facing app with SSO\n  on Enterprise. Each scheme below was observed or read on a provider page — none\n  is inferred from a spec.\n\napi_reference: null\napi_reference_note: >-\n  No OpenAPI, Swagger, GraphQL SDL or Postman collection is published on any\n  involve.me host. developers.involve.me\
  \ and docs.involve.me both return 302 to\n  the marketing homepage.\n\nschemes:\n\n  - id: mcp_oauth2\n    type: oauth2\n    surface: https://www-cdn.involve.me/mcp/statamic\n    applies_to: The Statamic CMS MCP server (marketing website content).\n    method: probed\n    flows:\n      authorization_code:\n        authorization_url: https://www-cdn.involve.me/cp/mcp/oauth/authorize\n        token_url: https://www-cdn.involve.me/mcp/oauth/token\n        refresh_supported: true\n        pkce: S256\n        pkce_required: true\n    dynamic_client_registration:\n      supported: true\n      registration_endpoint: https://www-cdn.involve.me/mcp/oauth/register\n      client_id_metadata_document_supported: true\n    revocation_endpoint: https://www-cdn.involve.me/mcp/oauth/revoke\n    token_endpoint_auth_methods: [none]\n    bearer_methods_supported: [header]\n    scopes: scopes/involve-me-scopes.yml\n    evidence:\n      url: https://www.involve.me/.well-known/oauth-authorization-server\n  \
  \    http_status: 200\n\n  - id: mcp_static_token\n    type: http\n    scheme: bearer\n    alternate: basic\n    surface: https://www-cdn.involve.me/mcp/statamic\n    applies_to: The same MCP server, as an alternative to the OAuth flow.\n    method: probed\n    detail: >-\n      The unauthenticated 401 body states \"Provide a Bearer token or Basic Auth\n      credentials\" and hints \"Create an API token in the Statamic MCP dashboard\" —\n      i.e. a tenant-issued static token created inside the CMS control panel. No\n      public documentation of that token's format, rotation or expiry exists.\n    evidence:\n      url: https://www-cdn.involve.me/mcp/statamic\n      http_status: 401\n      www_authenticate: Bearer realm=\"mcp\"\n\n  - id: webhook_custom_header\n    type: apiKey\n    in: header\n    surface: outbound webhook delivery\n    direction: outbound\n    applies_to: >-\n      involve.me POSTing submission data to the integrator's endpoint. involve.me\n      is the CLIENT here;\
  \ the integrator defines the credential.\n    method: searched\n    detail: >-\n      The webhook configuration accepts one custom \"Header Name\" / \"Header Value\"\n      pair, which involve.me sends on every delivery. This is the only\n      authentication available on the webhook surface.\n    name: user-defined\n    signature_verification: false\n    signature_note: >-\n      No HMAC signature, no signing secret and no timestamp header is documented.\n      A receiver cannot cryptographically verify that a payload came from\n      involve.me — a shared static header is the whole of the trust model.\n    evidence:\n      url: https://help.involve.me/en/articles/2193514-receive-submission-data-with-webhooks-anywhere\n      http_status: 200\n\n  - id: app_sso\n    type: openIdConnect\n    surface: https://app.involve.me/login\n    applies_to: Human sign-in to the involve.me application.\n    method: searched\n    detail: >-\n      Single sign-on is listed as an Enterprise-plan feature\
  \ on the pricing page.\n      The identity providers, protocol (SAML vs OIDC) and configuration are not\n      publicly documented; involve.me publishes no /.well-known/openid-configuration\n      (probed 404 on www. and app.).\n    evidence:\n      url: https://www.involve.me/pricing\n      http_status: 200\n\n  - id: app_session\n    type: http\n    scheme: cookie\n    surface: https://app.involve.me\n    applies_to: The product SPA's own backend.\n    method: probed\n    detail: >-\n      app.involve.me/api/v1/* returns 302 to login for anonymous callers and the\n      edge sets XSRF-TOKEN and lvapp_session cookies (Laravel). This is an internal,\n      session-authenticated surface, not a published API — it is recorded for\n      accuracy, not as an integration path.\n    evidence:\n      url: https://app.involve.me/api/v1/projects\n      http_status: 302\n\nsummary:\n  public_api_key_programme: false\n  oauth2: true\n  openid_connect_discovery: false\n  mtls: false\n  webhook_signature_verification:\
  \ false\n  scheme_count: 5\n\ngaps:\n  - >-\n    No published authentication documentation for developers of any kind — the\n    OAuth metadata is discoverable only by probing /.well-known/.\n  - >-\n    Webhook deliveries carry no signature. Adding an HMAC signature header with a\n    per-endpoint secret is the single highest-value authentication fix available\n    to involve.me.\n  - >-\n    Token lifetime, refresh-token rotation and expiry are not stated anywhere for\n    the MCP credential.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/involve-me/refs/heads/main/authentication/involve-me-authentication.yml
summary_line: 5 schemes
tags:
- Company
- Marketing
- Lead Generation
- Forms
- Surveys
- Quizzes
- No-Code
- Email Marketing
- CRM
- Webhooks
- Model Context Protocol
- Austria
---
