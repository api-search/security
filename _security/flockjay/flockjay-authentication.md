---
api_key_in: []
auth_types: []
description: Flockjay runs two authentication paths against one API host. Human/first-party clients use a DRF token ("Basic token authentication required" is the literal 401 body). Agents and third-party clients use OAuth 2.1 authorization-code + PKCE against api.flockjay.com, with dynamic client registration — this is the path the MCP server requires. There is no published developer portal, no key self-service page, and no OpenAPI securitySchemes block to derive from; every fact below was observed on the wire.
kind: authentication
layout: security
method: probed
name: Flockjay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flockjay declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Flockjay
provider_slug: flockjay
scheme_count: 2
schemes:
- applies_to: https://api.flockjay.com/api/
  evidence:
    body: '{"detail":"Basic token authentication required."}'
    http_status: 401
    url: https://api.flockjay.com/api/users/
  format: Token <token>
  header: Authorization
  id: drf-token
  in: header
  issuance: Not self-service. No public signup or key page was found; tokens appear to be issued to a provisioned Flockjay tenant.
  observed_variants:
  - body: '{"detail":"Basic token authentication required."}'
    seen_on:
    - /api/users/
    - /api/events/
    - /api/assignment_submissions/
    - /api/v2/user/
    - /api/v2/learning-content/
    - /api/v2/search/
    - /api/v2/sharedcontent/
    - /api/v2/event/
    - /api/v2/task/
    - /api/v2/user_certificate/
    - /api/v2/assignment-submission/
  - body: '{"detail":"Authentication credentials were not provided."}'
    note: Stock DRF message. Two different 401 bodies across sibling collections means the v1 surface mixes at least two permission/authentication classes.
    seen_on:
    - /api/questions/
    - /api/groups/
    - /api/module/
    - /api/submodule/
    - /api/rubrics/
    - /api/assignments/
    - /api/live_sessions/
  scheme: token
  type: http
- applies_to: https://api.flockjay.com/mcp
  authorization_endpoint: https://flockjay.com/oauth/authorize
  dcr_spec: RFC 7591
  dynamic_client_registration: true
  evidence:
    http_status: 200
    url: https://api.flockjay.com/.well-known/oauth-authorization-server
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  id: oauth2-authorization-code
  id_token_signing_alg:
  - RS256
  issuer: https://api.flockjay.com
  jwks_uri: https://api.flockjay.com/oauth/.well-known/jwks.json
  pkce: S256
  pkce_required: true
  registration_endpoint: https://api.flockjay.com/oauth/register/
  response_types:
  - code
  revocation_endpoint: https://api.flockjay.com/oauth/revoke/
  scopes:
  - read
  - offline_access
  subject_types:
  - public
  token_endpoint: https://api.flockjay.com/oauth/token/
  token_endpoint_auth_methods:
  - none
  type: oauth2
slug: flockjay-authentication
source_filename: flockjay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: >-\n  https://api.flockjay.com/.well-known/openid-configuration,\n  https://api.flockjay.com/.well-known/oauth-protected-resource, and live\n  unauthenticated probes of the Django REST Framework collections under\n  https://api.flockjay.com/api/ on 2026-08-14.\nname: Flockjay authentication profile\ndescription: >-\n  Flockjay runs two authentication paths against one API host. Human/first-party\n  clients use a DRF token (\"Basic token authentication required\" is the literal\n  401 body). Agents and third-party clients use OAuth 2.1 authorization-code +\n  PKCE against api.flockjay.com, with dynamic client registration — this is the\n  path the MCP server requires. There is no published developer portal, no key\n  self-service page, and no OpenAPI securitySchemes block to derive from; every\n  fact below was observed on the wire.\n\nschemes:\n- id: drf-token\n  type: http\n  scheme: token\n  in: header\n  header: Authorization\n\
  \  format: 'Token <token>'\n  applies_to: https://api.flockjay.com/api/\n  issuance: >-\n    Not self-service. No public signup or key page was found; tokens appear to be\n    issued to a provisioned Flockjay tenant.\n  evidence:\n    url: https://api.flockjay.com/api/users/\n    http_status: 401\n    body: '{\"detail\":\"Basic token authentication required.\"}'\n  observed_variants:\n  - body: '{\"detail\":\"Basic token authentication required.\"}'\n    seen_on:\n    - /api/users/\n    - /api/events/\n    - /api/assignment_submissions/\n    - /api/v2/user/\n    - /api/v2/learning-content/\n    - /api/v2/search/\n    - /api/v2/sharedcontent/\n    - /api/v2/event/\n    - /api/v2/task/\n    - /api/v2/user_certificate/\n    - /api/v2/assignment-submission/\n  - body: '{\"detail\":\"Authentication credentials were not provided.\"}'\n    seen_on:\n    - /api/questions/\n    - /api/groups/\n    - /api/module/\n    - /api/submodule/\n    - /api/rubrics/\n    - /api/assignments/\n    - /api/live_sessions/\n\
  \    note: >-\n      Stock DRF message. Two different 401 bodies across sibling collections means\n      the v1 surface mixes at least two permission/authentication classes.\n\n- id: oauth2-authorization-code\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  pkce_required: true\n  authorization_endpoint: https://flockjay.com/oauth/authorize\n  token_endpoint: https://api.flockjay.com/oauth/token/\n  revocation_endpoint: https://api.flockjay.com/oauth/revoke/\n  registration_endpoint: https://api.flockjay.com/oauth/register/\n  jwks_uri: https://api.flockjay.com/oauth/.well-known/jwks.json\n  issuer: https://api.flockjay.com\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  token_endpoint_auth_methods:\n  - none\n  scopes:\n  - read\n  - offline_access\n  id_token_signing_alg:\n  - RS256\n  subject_types:\n  - public\n  applies_to: https://api.flockjay.com/mcp\n  dynamic_client_registration: true\n  dcr_spec: RFC 7591\n  evidence:\n   \
  \ url: https://api.flockjay.com/.well-known/oauth-authorization-server\n    http_status: 200\n\nanonymous_surfaces:\n- path: /api/\n  http_status: 200\n  note: >-\n    Browsable DRF API root. Returns a JSON map of 20 collection URLs. The only\n    self-describing thing Flockjay publishes about its REST API.\n- path: /api/course/\n  http_status: 200\n  note: >-\n    Returns an empty paginated envelope {\"count\":0,...} without credentials. Reads\n    as an unauthenticated-but-tenant-scoped-to-nothing response rather than an open\n    collection.\n- path: /api/v2/sharedcontent/{linkId}/\n  http_status: 200\n  note: >-\n    Public share links resolve anonymously — this is the product feature behind\n    flockjay.com/share?linkId=..., including the link the Trust Center page uses to\n    serve its own PDF. Payload not captured here (contains named individuals).\n\nnotes:\n- >-\n  token_endpoint_auth_methods_supported is [\"none\"], i.e. public clients only. Paired\n  with mandatory PKCE and\
  \ dynamic client registration, this is a correctly-shaped\n  OAuth 2.1 public-client profile for agent use.\n- >-\n  The discovery document is served at BOTH /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server with identical bytes, but scopes_supported\n  does not include \"openid\" and there is no userinfo_endpoint — so it advertises\n  OIDC-shaped metadata without being a usable OIDC provider. Recorded as a deviation,\n  not as OIDC conformance.\n- >-\n  No API key scheme, no mTLS, no HMAC request signing was observed or documented.\n- >-\n  No public documentation of any of this exists. Flockjay publishes no auth guide,\n  no developer portal, and no OpenAPI. An integrator can only learn this by probing\n  the host, which is what API Evangelist did.\n\nrelated:\n  scopes: scopes/flockjay-scopes.yml\n  well_known: well-known/flockjay-well-known.yml\n  mcp: mcp/flockjay-mcp.yml\n  conventions: conventions/flockjay-conventions.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flockjay/refs/heads/main/authentication/flockjay-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Sales Enablement
- Sales Training
- Learning Management
- Revenue Operations
- AI Coaching
- Content Management
- Software-as-a-Service
- MCP
- Agent Native
- Authentication
---
