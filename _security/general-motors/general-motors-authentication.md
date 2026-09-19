---
anonymous_access: false
api_key_in: []
auth_types: []
description: General Motors publishes no authentication documentation for its connected-vehicle / fleet APIs — the reference that would describe it sits behind the portal's commercial-access gate. What IS publicly verifiable is how the GM Developer Portal's own API backend authenticates, established here by probe rather than by documentation.
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: General Motors Authentication
name_suffix: Authentication
oauth_flows: []
overview: General Motors declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: General Motors
provider_slug: general-motors
scheme_count: 2
schemes:
- applies_to: https://developer.gm.com/v1 (GM Developer Portal backend)
  bearer: 'Authorization: Bearer <id token>'
  client_id: def7864f-a5b6-4d80-b024-592df723ad5a
  flow: authorization_code (MSAL browser client, PKCE)
  id: entra-external-id-bearer
  identity_provider: Microsoft Entra External ID (CIAM)
  issuer: https://450fd55c-b136-4d90-9e9f-a59b07772fab.ciamlogin.com/450fd55c-b136-4d90-9e9f-a59b07772fab/v2.0
  jwks_uri: https://450fd55c-b136-4d90-9e9f-a59b07772fab.ciamlogin.com/450fd55c-b136-4d90-9e9f-a59b07772fab/discovery/v2.0/keys
  ownership_note: The issuer is a Microsoft-hosted CIAM host, not a GM host. It is attributed to GM because developer.gm.com serves the tenant id, client id and redirect URI itself, unauthenticated, from its own /config/index.js — the portal names this tenant as its authority.
  redirect_uri: https://developer.gm.com/
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  token_endpoint: https://450fd55c-b136-4d90-9e9f-a59b07772fab.ciamlogin.com/450fd55c-b136-4d90-9e9f-a59b07772fab/oauth2/v2.0/token
  type: oauth2
- anonymous: true
  applies_to: https://developer.gm.com/v1 (state-changing requests)
  header: X-XSRF-TOKEN
  id: csrf-double-submit
  note: GET /v1/csrf-token answers 200 anonymously and returns {audience, token, headerName}. It is the only endpoint under /v1 that answers without a bearer token.
  token_endpoint: https://developer.gm.com/v1/csrf-token
  type: csrf
slug: general-motors-authentication
source_filename: general-motors-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication Profile\nspecificationVersion: '0.1'\nprovider: General Motors\nproviderId: general-motors\ngenerated: '2026-09-12'\nmethod: probed\nsource: https://developer.gm.com/config/index.js\ndescription: >-\n  General Motors publishes no authentication documentation for its connected-vehicle / fleet\n  APIs — the reference that would describe it sits behind the portal's commercial-access\n  gate. What IS publicly verifiable is how the GM Developer Portal's own API backend\n  authenticates, established here by probe rather than by documentation.\nscoring_note: >-\n  NO `Authentication` pointer is wired into apis.yml for this file, on purpose. The rating's\n  authentication_documented check asserts that the PROVIDER documents authentication for its\n  API; GM does not. This artifact records what we were able to observe, not a published auth\n  guide, and crediting it would be a false claim made on GM's behalf.\nschemes:\n- id: entra-external-id-bearer\n\
  \  type: oauth2\n  applies_to: https://developer.gm.com/v1 (GM Developer Portal backend)\n  flow: authorization_code (MSAL browser client, PKCE)\n  identity_provider: Microsoft Entra External ID (CIAM)\n  issuer: https://450fd55c-b136-4d90-9e9f-a59b07772fab.ciamlogin.com/450fd55c-b136-4d90-9e9f-a59b07772fab/v2.0\n  client_id: def7864f-a5b6-4d80-b024-592df723ad5a\n  redirect_uri: https://developer.gm.com/\n  scopes_supported:\n  - openid\n  - profile\n  - email\n  - offline_access\n  token_endpoint: https://450fd55c-b136-4d90-9e9f-a59b07772fab.ciamlogin.com/450fd55c-b136-4d90-9e9f-a59b07772fab/oauth2/v2.0/token\n  jwks_uri: https://450fd55c-b136-4d90-9e9f-a59b07772fab.ciamlogin.com/450fd55c-b136-4d90-9e9f-a59b07772fab/discovery/v2.0/keys\n  bearer: 'Authorization: Bearer <id token>'\n  ownership_note: >-\n    The issuer is a Microsoft-hosted CIAM host, not a GM host. It is attributed to GM because\n    developer.gm.com serves the tenant id, client id and redirect URI itself, unauthenticated,\n\
  \    from its own /config/index.js — the portal names this tenant as its authority.\n- id: csrf-double-submit\n  type: csrf\n  applies_to: https://developer.gm.com/v1 (state-changing requests)\n  header: X-XSRF-TOKEN\n  token_endpoint: https://developer.gm.com/v1/csrf-token\n  anonymous: true\n  note: >-\n    GET /v1/csrf-token answers 200 anonymously and returns {audience, token, headerName}.\n    It is the only endpoint under /v1 that answers without a bearer token.\nauthorization:\n  model: commercial-agreement\n  note: >-\n    Signing in is not sufficient. The portal's router guards /docs/* with\n    requireCommercialAPIAccess, so the API reference is released per-account only after GM\n    approves commercial API access.\nobserved:\n- url: https://developer.gm.com/v1/csrf-token\n  method: GET\n  status: 200\n  detail: anonymous; returns the CSRF token envelope\n- url: https://developer.gm.com/v1/apis\n  method: GET\n  status: 403\n  detail: empty body, istio-envoy upstream — bearer\
  \ token required\n- url: https://developer.gm.com/v1/graphql\n  method: POST\n  status: 403\n  detail: '{\"message\":\"Invalid or missing CSRF token. Call GET /v1/csrf-token first.\",\"error\":\"CSRF_VALIDATION_FAILED\"}'\n- url: https://450fd55c-b136-4d90-9e9f-a59b07772fab.ciamlogin.com/450fd55c-b136-4d90-9e9f-a59b07772fab/v2.0/.well-known/openid-configuration\n  method: GET\n  status: 200\n  detail: OpenID Provider Metadata for the tenant the portal signs in against\nunknown:\n- The authentication model for the OnStar / GM Envolve vehicle-data and fleet APIs\n  (api.gm.com, api.onstarfleetintelligence.com) is not publicly documented.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/general-motors/refs/heads/main/authentication/general-motors-authentication.yml
summary_line: 2 schemes
tags:
- Automobiles
- Cars
- Vehicles
- Connected Vehicles
- Telematics
- Fortune 100
---
