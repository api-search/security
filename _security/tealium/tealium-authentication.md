---
api_key_in: []
api_specs:
- filename: tealium-auth-api-openapi.yml
  format: yaml
  label: Tealium Auth API
  slug: tealium-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-auth-api-openapi.yml
- filename: tealium-collect-api-openapi.yml
  format: yaml
  label: Tealium Collect API
  slug: tealium-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-collect-api-openapi.yml
- filename: tealium-customer-api-openapi.yml
  format: yaml
  label: Tealium Customer API
  slug: tealium-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-customer-api-openapi.yml
- filename: tealium-personalization-api-openapi.yml
  format: yaml
  label: Tealium Personalization API
  slug: tealium-personalization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-personalization-api-openapi.yml
- filename: tealium-privacy-api-openapi.yml
  format: yaml
  label: Tealium Privacy API
  slug: tealium-privacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-privacy-api-openapi.yml
- filename: tealium-wp-json-api-openapi.yml
  format: yaml
  label: Tealium Wp Json API
  slug: tealium-wp-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/openapi/tealium-wp-json-api-openapi.yml
auth_types:
- http
- apiKey
- none
description: Tealium runs four different authentication models across one platform, and which one applies depends on the product rather than the version. The V3 platform APIs use a short-lived JWT exchanged from an API key; SCIM uses a 90-day long-lived token from a different host; the Moments API uses no credential at all and is governed by a domain allowlist; the managed MCP server uses a dedicated static API-key header. There is no OAuth 2.0 and no OpenID Connect anywhere.
kind: authentication
layout: security
method: searched
name: Tealium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tealium secures its APIs with http, apiKey, and none across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tealium
provider_slug: tealium
scheme_count: 4
schemes:
- applies_to:
  - Tealium Collect HTTP API
  - Tealium Visitor Profile API
  - Tealium Visitor Privacy API
  - Tealium iQ Profiles API
  bearerFormat: JWT
  description: JWT bearer token obtained from the Authentication API (POST /v3/auth/accounts/{account}/profiles/{profile}). Tokens are valid for 30 minutes. Do not generate a new token for every call — reuse until expiration or Tealium will throttle the authentication endpoint at its discretion.
  name: BearerAuth
  obtained_by:
    content_type: application/x-www-form-urlencoded
    endpoint: POST https://platform.tealiumapis.com/v3/auth/accounts/{account}/profiles/{profile}
    parameters:
    - description: The Tealium user's email address, URL-encoded.
      name: username
    - description: An API key generated in Tealium iQ, URL-encoded, used in place of a password.
      name: key
    response_fields:
    - description: The JWT bearer token.
      name: token
    - description: The region-specific host that all subsequent region-specific calls must use, e.g. us-east-1-platform.tealiumapis.com. Ignoring this field is the most common integration error on the platform.
      name: host
  scheme: bearer
  sources:
  - openapi/_original/tealium-collect-http-openapi.yml
  - openapi/_original/tealium-visitor-privacy-openapi.yml
  - openapi/_original/tealium-visitor-profile-openapi.yml
  ttl_seconds: 1800
  type: http
- applies_to:
  - Tealium SCIM API
  bearerFormat: JWT
  description: A 90-day bearer token for identity-provider integrations, minted from the same username + API key pair but on a different host. Tealium describes it as "the OAuth bearer token" for provisioning applications, though no OAuth grant is involved.
  guidance: Tealium recommends minting this from a dedicated service user (for example scim@example.com) rather than a person's account, so the integration survives that person's departure.
  name: LongLivedBearer
  obtained_by:
    content_type: application/x-www-form-urlencoded
    endpoint: POST https://developer.tealiumapis.com/v2/auth-long-lived/token
    parameters:
    - account
    - profile
    - username
    - key
    rate_limit: 10 requests per minute per IP address
  revocation:
    endpoint: POST https://developer.tealiumapis.com/v2/auth-long-lived/revoke
    parameters:
    - token
    - account
    - profile
    - username
    - key
    - token_type_hint
    rate_limit: 20 requests per minute per IP address
    semantics: Immediate and permanent, effective within seconds and not undoable. Returns 200 whether or not the token was already expired or revoked; 401 means the supplied credentials do not match the credentials used to mint the token.
  scheme: bearer
  scope_string: profile email
  ttl_seconds: 7776000
  type: http
- applies_to:
  - Tealium Moments API
  boundary: Each engine defines exactly which audiences, badges and attributes are returned, capped at 1 kB per visitor per engine, maximum 10 engines per profile.
  description: No credential. Access is governed by an allowlist of domains configured on the Moments API engine, plus mandatory Origin and Referer headers on every request. This is what makes the Moments API callable from a browser without exposing a secret — and what makes the engine configuration, not a token, the access-control boundary.
  name: MomentsDomainAllowlist
  required_headers:
  - Origin
  - Referer
  type: none
- applies_to:
  - Moments API managed MCP server
  description: A dedicated static API key issued by Tealium Support specifically for managed MCP server access. It is not the standard Tealium iQ API key and not a V3 JWT. Origin and Referer headers are also required.
  endpoint: https://us-west-2.prod.developer.tealiumapis.com/v1/personalization/mcp
  header_name: X-Tealium-Api-Key
  in: header
  name: TealiumMcpApiKey
  oauth_metadata: No /.well-known/oauth-protected-resource (RFC 9728) and no /.well-known/oauth-authorization-server (RFC 8414) on the MCP host — both 404. This server does not implement the MCP OAuth authorization flow.
  probed:
    body: '{"message":"Unauthorized","http_status_code":401}'
    date: '2026-08-13'
    http_status: 401
    method: POST tools/list without the header
  provisioning: request from Tealium Support
  type: apiKey
slug: tealium-authentication
source_filename: tealium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/_original/*.yml (securitySchemes) + Tealium's own authentication documentation\ndocs:\n  - https://docs.tealium.com/api/v3/getting-started/authentication/\n  - https://docs.tealium.com/api/v2/getting-started/auth/\n  - https://docs.tealium.com/administration/security-access/api-keys/\n  - https://docs.tealium.com/api/v3/scim-api/about/\n  - https://docs.tealium.com/server-side/moments-api/managed-mcp-server/\ndescription: >-\n  Tealium runs four different authentication models across one platform, and which one applies\n  depends on the product rather than the version. The V3 platform APIs use a short-lived JWT\n  exchanged from an API key; SCIM uses a 90-day long-lived token from a different host; the Moments\n  API uses no credential at all and is governed by a domain allowlist; the managed MCP server uses\n  a dedicated static API-key header. There is no OAuth 2.0 and no OpenID Connect anywhere.\n\nsummary:\n  types:\n\
  \    - http\n    - apiKey\n    - none\n  oauth2: false\n  oidc: false\n  mtls: false\n  scopes: false\n  scopes_note: >-\n    No OAuth scope surface exists. Authorization is by Tealium permission groups and admin roles\n    attached to the user who generated the key, not by token scope. The long-lived SCIM token\n    returns a scope string of \"profile email\" but no scope is ever requested or enforced.\n\nschemes:\n  - name: BearerAuth\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to:\n      - Tealium Collect HTTP API\n      - Tealium Visitor Profile API\n      - Tealium Visitor Privacy API\n      - Tealium iQ Profiles API\n    description: >-\n      JWT bearer token obtained from the Authentication API\n      (POST /v3/auth/accounts/{account}/profiles/{profile}). Tokens are valid for 30 minutes. Do\n      not generate a new token for every call — reuse until expiration or Tealium will throttle the\n      authentication endpoint at its discretion.\n    ttl_seconds:\
  \ 1800\n    obtained_by:\n      endpoint: POST https://platform.tealiumapis.com/v3/auth/accounts/{account}/profiles/{profile}\n      content_type: application/x-www-form-urlencoded\n      parameters:\n        - name: username\n          description: The Tealium user's email address, URL-encoded.\n        - name: key\n          description: An API key generated in Tealium iQ, URL-encoded, used in place of a password.\n      response_fields:\n        - name: token\n          description: The JWT bearer token.\n        - name: host\n          description: >-\n            The region-specific host that all subsequent region-specific calls must use, e.g.\n            us-east-1-platform.tealiumapis.com. Ignoring this field is the most common integration\n            error on the platform.\n    sources:\n      - openapi/_original/tealium-collect-http-openapi.yml\n      - openapi/_original/tealium-visitor-privacy-openapi.yml\n      - openapi/_original/tealium-visitor-profile-openapi.yml\n\n  -\
  \ name: LongLivedBearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    applies_to:\n      - Tealium SCIM API\n    description: >-\n      A 90-day bearer token for identity-provider integrations, minted from the same username + API\n      key pair but on a different host. Tealium describes it as \"the OAuth bearer token\" for\n      provisioning applications, though no OAuth grant is involved.\n    ttl_seconds: 7776000\n    scope_string: 'profile email'\n    obtained_by:\n      endpoint: POST https://developer.tealiumapis.com/v2/auth-long-lived/token\n      content_type: application/x-www-form-urlencoded\n      parameters: [account, profile, username, key]\n      rate_limit: 10 requests per minute per IP address\n    revocation:\n      endpoint: POST https://developer.tealiumapis.com/v2/auth-long-lived/revoke\n      parameters: [token, account, profile, username, key, token_type_hint]\n      rate_limit: 20 requests per minute per IP address\n      semantics: >-\n      \
  \  Immediate and permanent, effective within seconds and not undoable. Returns 200 whether or\n        not the token was already expired or revoked; 401 means the supplied credentials do not\n        match the credentials used to mint the token.\n    guidance: >-\n      Tealium recommends minting this from a dedicated service user (for example scim@example.com)\n      rather than a person's account, so the integration survives that person's departure.\n\n  - name: MomentsDomainAllowlist\n    type: none\n    applies_to:\n      - Tealium Moments API\n    description: >-\n      No credential. Access is governed by an allowlist of domains configured on the Moments API\n      engine, plus mandatory Origin and Referer headers on every request. This is what makes the\n      Moments API callable from a browser without exposing a secret — and what makes the engine\n      configuration, not a token, the access-control boundary.\n    required_headers: [Origin, Referer]\n    boundary: >-\n      Each\
  \ engine defines exactly which audiences, badges and attributes are returned, capped at\n      1 kB per visitor per engine, maximum 10 engines per profile.\n\n  - name: TealiumMcpApiKey\n    type: apiKey\n    in: header\n    header_name: X-Tealium-Api-Key\n    applies_to:\n      - Moments API managed MCP server\n    description: >-\n      A dedicated static API key issued by Tealium Support specifically for managed MCP server\n      access. It is not the standard Tealium iQ API key and not a V3 JWT. Origin and Referer\n      headers are also required.\n    endpoint: https://us-west-2.prod.developer.tealiumapis.com/v1/personalization/mcp\n    provisioning: request from Tealium Support\n    probed:\n      method: 'POST tools/list without the header'\n      http_status: 401\n      body: '{\"message\":\"Unauthorized\",\"http_status_code\":401}'\n      date: '2026-08-13'\n    oauth_metadata: >-\n      No /.well-known/oauth-protected-resource (RFC 9728) and no\n      /.well-known/oauth-authorization-server\
  \ (RFC 8414) on the MCP host — both 404. This server\n      does not implement the MCP OAuth authorization flow.\n\napi_keys:\n  management: https://docs.tealium.com/administration/security-access/api-keys/\n  scoping: 'Per user, per account/profile, governed by Tealium permission groups and admin roles.'\n  test_keys: false\n  test_keys_note: There is no test-vs-live key distinction. See sandbox/tealium-sandbox.yml.\n  rotation: >-\n    No documented automatic rotation or expiry for the underlying API key. Only the derived tokens\n    expire (30 minutes for V3, 90 days for long-lived).\n\naccount_security:\n  sso:\n    protocol: SAML 2.0\n    idps: [ADFS (Active Directory), Azure, Okta]\n    certificate_status_monitoring: true\n    docs: https://docs.tealium.com/administration/security-access/single-sign-on/sso/\n  mfa:\n    supported: true\n    docs: https://docs.tealium.com/administration/security-access/multi-factor-authentication-mfa/\n  password_policy: https://docs.tealium.com/administration/security-access/password-policy/\n\
  \  session_timeout: https://docs.tealium.com/administration/security-access/session-timeout/\n  ip_allowlist: https://docs.tealium.com/administration/security-access/ip-allow-list/\n  scim_provisioning: https://docs.tealium.com/api/v3/scim-api/about/\n\ngaps:\n  - No OAuth 2.0 authorization flow and no OpenID Connect discovery.\n  - No token scopes — a V3 JWT carries the full permissions of the user who minted it.\n  - No documented API-key rotation policy or key expiry.\n  - No test-mode credentials.\n  - The MCP server's static header key cannot be scoped, rotated per client, or short-lived.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tealium/refs/heads/main/authentication/tealium-authentication.yml
summary_line: http/apiKey/none · 4 schemes
tags:
- Customer Data Platform
- CDP
- Tag Management
- AudienceStream
- Real-Time Events
- Visitor Profiles
- Audience Segmentation
- Data Collection
- Privacy Compliance
- Personalization
---
