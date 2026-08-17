---
api_key_in: []
api_specs:
- filename: pavoot-api-openapi.json
  format: json
  label: Pavoot Application API
  slug: pavoot-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pavoot/refs/heads/main/openapi/pavoot-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Pavoot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pavoot declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Pavoot
provider_slug: pavoot
scheme_count: 2
schemes:
- bearer_format: JWT
  declared_in_spec: false
  description: Clerk-issued session JWT. Verified against the Pavoot Clerk instance (issuer https://clerk.pavoot.com, RS256, JWKS at https://clerk.pavoot.com/.well-known/jwks.json). The GET /me operation documents that "Clerk is shared across multiple Pavoot apps, so a valid Clerk session does NOT imply the user belongs here" — app membership is resolved from this application's own database, not from Clerk public_metadata.
  evidence:
    body: '{"detail":"Unauthorized: Authentication failed"}'
    http_status: 401
    url: https://api.pavoot.com/me
  header: Authorization
  id: clerk_session_bearer
  in: header
  scheme: bearer
  type: http
- authorization_endpoint: https://clerk.pavoot.com/oauth/authorize
  description: Pavoot runs a Clerk-hosted OAuth 2.0 / OpenID Connect authorization server on its own subdomain. Discovery is anonymous and returns a real RFC 8414 / OIDC document. This is the identity layer behind the app; Pavoot does not publish a developer OAuth client-registration flow.
  evidence:
    content_type: application/json
    http_status: 200
    url: https://clerk.pavoot.com/.well-known/openid-configuration
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  id: clerk_oauth2
  introspection_endpoint: https://clerk.pavoot.com/oauth/token_info
  issuer: https://clerk.pavoot.com
  jwks_uri: https://clerk.pavoot.com/.well-known/jwks.json
  pkce: S256
  revocation_endpoint: https://clerk.pavoot.com/oauth/token/revoke
  token_endpoint: https://clerk.pavoot.com/oauth/token
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: oauth2
  userinfo_endpoint: https://clerk.pavoot.com/oauth/userinfo
slug: pavoot-authentication
source_filename: pavoot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  https://api.pavoot.com/openapi.json (no securitySchemes declared) +\n  https://api.pavoot.com/me (401 probe) +\n  https://clerk.pavoot.com/.well-known/openid-configuration\nname: Pavoot Application API authentication\nsummary: >-\n  Pavoot's application API at api.pavoot.com is authenticated with Clerk-issued\n  session tokens presented as a bearer credential. The published OpenAPI declares\n  NO components.securitySchemes and NO operation-level security, so the auth model\n  below was established by probing the live API and Pavoot's own Clerk OIDC\n  discovery document — not read from the spec.\nschemes:\n- id: clerk_session_bearer\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  in: header\n  header: Authorization\n  description: >-\n    Clerk-issued session JWT. Verified against the Pavoot Clerk instance\n    (issuer https://clerk.pavoot.com, RS256, JWKS at\n    https://clerk.pavoot.com/.well-known/jwks.json).\
  \ The GET /me operation\n    documents that \"Clerk is shared across multiple Pavoot apps, so a valid\n    Clerk session does NOT imply the user belongs here\" — app membership is\n    resolved from this application's own database, not from Clerk\n    public_metadata.\n  declared_in_spec: false\n  evidence:\n    url: https://api.pavoot.com/me\n    http_status: 401\n    body: '{\"detail\":\"Unauthorized: Authentication failed\"}'\n- id: clerk_oauth2\n  type: oauth2\n  flow: authorization_code\n  pkce: S256\n  issuer: https://clerk.pavoot.com\n  authorization_endpoint: https://clerk.pavoot.com/oauth/authorize\n  token_endpoint: https://clerk.pavoot.com/oauth/token\n  introspection_endpoint: https://clerk.pavoot.com/oauth/token_info\n  revocation_endpoint: https://clerk.pavoot.com/oauth/token/revoke\n  userinfo_endpoint: https://clerk.pavoot.com/oauth/userinfo\n  jwks_uri: https://clerk.pavoot.com/.well-known/jwks.json\n  grant_types:\n  - authorization_code\n  - refresh_token\n  token_endpoint_auth_methods:\n\
  \  - client_secret_basic\n  - client_secret_post\n  - none\n  description: >-\n    Pavoot runs a Clerk-hosted OAuth 2.0 / OpenID Connect authorization server on\n    its own subdomain. Discovery is anonymous and returns a real RFC 8414 / OIDC\n    document. This is the identity layer behind the app; Pavoot does not publish a\n    developer OAuth client-registration flow.\n  evidence:\n    url: https://clerk.pavoot.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\nunauthenticated_surfaces:\n- path: /openapi.json\n  note: The FastAPI-generated OpenAPI document is served publicly with no auth.\n  http_status: 200\n- path: /docs\n  note: FastAPI Swagger UI, publicly reachable.\n  http_status: 200\n- path: /redoc\n  note: FastAPI ReDoc, publicly reachable.\n  http_status: 200\n- path: /attendee-registration-info/{token}\n  note: >-\n    Explicitly public per its own description (\"Public: returns project name and\n    layout for the registration\
  \ form. No auth required.\") — token-scoped, not\n    session-scoped.\n- path: /register-attendee\n  note: >-\n    Accepts a public registration token for attendee self-registration; the\n    member-token variant requires a signed-in Clerk user.\n- path: /upload-link-by-token\n  note: Upload-link token surface, resolved by opaque token rather than session.\nauthorization:\n  model: >-\n    Fine-grained, database-backed RBAC layered on top of the Clerk session. The API\n    exposes an explicit permission surface rather than OAuth scopes: role and user\n    permission matrices, permission presets with a settable default, per-task\n    permissions, and a middleware helper.\n  surfaces:\n  - operationId: check_route_access_endpoint_checkRouteAccess_get\n    path: /checkRouteAccess\n    note: >-\n      Returns {\"allowed\": true|false} for the current user and a given path; used\n      by the frontend middleware to gate /faces, /personalized-tags,\n      /photographers, /recipients.\n  - operationId:\
  \ get_effective_permissions_endpoint_getEffectivePermissions_get\n    path: /getEffectivePermissions\n  - operationId: get_effective_org_permissions_endpoint_getEffectiveOrgPermissions_get\n    path: /getEffectiveOrgPermissions\n  - path: /org/permissions/role-matrix\n  - path: /org/permissions/user-matrix\n  - path: /org/permission-presets\n  - path: /admin/isAdmin\n  tenancy: >-\n    Two-level tenancy — organization (organizationId) and project (projectId).\n    Nearly every read operation is scoped by a required projectId or\n    organizationId query parameter; admin/* operations are gated on a separate\n    platform-admin check.\ndeveloper_access:\n  public_signup: false\n  api_keys: false\n  note: >-\n    Pavoot publishes no developer program, no API key issuance, and no partner\n    OAuth client registration. Credentials are obtained by being a user of the\n    Pavoot application, not by registering as an API consumer. The OpenAPI is\n    readable by anyone; the API itself is not\
  \ callable by anyone.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pavoot/refs/heads/main/authentication/pavoot-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Events
- Event Management
- Marketing
- AI Agent
- Attendee Intelligence
- GTM
- Field Marketing
- Pipeline
---
