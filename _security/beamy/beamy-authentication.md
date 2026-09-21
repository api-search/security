---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication profile observed at the edge. Beamy publishes no OpenAPI and no public auth reference, so this records only what the hosts themselves assert to an anonymous caller.
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Beamy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Beamy declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Beamy
provider_slug: beamy
scheme_count: 2
schemes:
- detail: Kong's key-auth plugin fronts every path on api.beamy.io. The plugin accepts the key in a header or query parameter whose name is configured per gateway; Beamy does not publish which name it uses, so the parameter name is recorded as unknown rather than assumed.
  docs: null
  host: api.beamy.io
  id: kong-key-auth
  key_location: unknown
  key_parameter: unknown
  observed:
    body: '{"message":"No API key found in request","request_id":"..."}'
    server: kong/3.9.3
    status: 401
    www_authenticate: Key
  self_service_keys: false
  type: apiKey
- detail: Internal client API called by the app.beamy.io single-page app; TOKEN_EMPTY indicates a bearer token issued by the app's login flow (auth.beamy.io is a Firebase-hosted login page). Not a public integration surface.
  host: clientapi.prod.beamy.io
  id: bearer-token
  observed:
    body: '{"statusCode":401,"message":"TOKEN_EMPTY"}'
    status: 401
  scheme: bearer
  type: http
slug: beamy-authentication
source_filename: beamy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: probed\nsource:\n- https://api.beamy.io/\n- https://clientapi.prod.beamy.io/\n- https://app.beamy.io/\n- https://auth.beamy.io/\nprovider: Beamy\nproviderId: beamy\ndescription: >-\n  Authentication profile observed at the edge. Beamy publishes no OpenAPI and no public auth\n  reference, so this records only what the hosts themselves assert to an anonymous caller.\nschemes:\n- id: kong-key-auth\n  type: apiKey\n  host: api.beamy.io\n  observed:\n    status: 401\n    www_authenticate: Key\n    body: '{\"message\":\"No API key found in request\",\"request_id\":\"...\"}'\n    server: kong/3.9.3\n  detail: >-\n    Kong's key-auth plugin fronts every path on api.beamy.io. The plugin accepts the key in a\n    header or query parameter whose name is configured per gateway; Beamy does not publish which\n    name it uses, so the parameter name is recorded as unknown rather than assumed.\n  key_parameter: unknown\n  key_location: unknown\n  self_service_keys:\
  \ false\n  docs: null\n- id: bearer-token\n  type: http\n  scheme: bearer\n  host: clientapi.prod.beamy.io\n  observed:\n    status: 401\n    body: '{\"statusCode\":401,\"message\":\"TOKEN_EMPTY\"}'\n  detail: >-\n    Internal client API called by the app.beamy.io single-page app; TOKEN_EMPTY indicates a bearer\n    token issued by the app's login flow (auth.beamy.io is a Firebase-hosted login page). Not a\n    public integration surface.\noauth2: null\nopenid_configuration: null\nmutual_tls: false\nsso:\n  detail: >-\n    The product integrates with Okta and Azure AD for SSO (apis.yml Integrations); the identity\n    provider metadata is not published on any Beamy host — /.well-known/openid-configuration 404s\n    on auth.beamy.io and is key-gated on api.beamy.io.\nhow_to_get_credentials: >-\n  No public path. Keys are issued to customers; the implementation documentation is behind the\n  docs.beamy.io lead form (email, name, company) and the full library behind a Beamy account.\nx-evidence:\n\
  - url: https://api.beamy.io/\n  http_status: 401\n  fetched: '2026-09-18'\n- url: https://clientapi.prod.beamy.io/\n  http_status: 401\n  fetched: '2026-09-18'\n- url: https://auth.beamy.io/.well-known/openid-configuration\n  http_status: 404\n  fetched: '2026-09-18'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/beamy/refs/heads/main/authentication/beamy-authentication.yml
summary_line: 2 schemes
tags:
- SaaS Management
- Shadow IT
- IT Asset Management
- Cloud Governance
- Security
- Application Portfolio Management
- Usage Analytics
- AI Governance
---
