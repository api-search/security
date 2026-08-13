---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Paramark Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paramark declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Paramark
provider_slug: paramark
scheme_count: 0
schemes: []
slug: paramark-authentication
source_filename: paramark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: https://signin.paramark.com/.well-known/openid-configuration\ndocs: https://paramark.com/pricing\nnote: >-\n  Paramark publishes no public API reference, so this profile is built from what its own hosts\n  return anonymously rather than from an OpenAPI securitySchemes block. Two authentication\n  surfaces were observed directly: a full OpenID Connect / OAuth 2.0 authorization server at\n  signin.paramark.com (documents saved verbatim under well-known/), and an HTTP Basic challenge\n  guarding the API host's own contract at api.paramark.com. No OpenAPI document was recoverable,\n  so nothing below is derived from a spec — every field is read from a live response.\nsurfaces:\n- name: Paramark identity (OIDC / OAuth 2.0)\n  host: signin.paramark.com\n  issuer: https://signin.paramark.com\n  type: openIdConnect\n  discovery: https://signin.paramark.com/.well-known/openid-configuration\n  authorization_server_metadata: https://signin.paramark.com/.well-known/oauth-authorization-server\n\
  \  jwks_uri: https://signin.paramark.com/oauth2/jwks\n  platform: WorkOS AuthKit, on Paramark's own custom domain (the served document's\n    issuer is https://signin.paramark.com)\n  endpoints:\n    authorization: https://signin.paramark.com/oauth2/authorize\n    token: https://signin.paramark.com/oauth2/token\n    userinfo: https://signin.paramark.com/oauth2/userinfo\n    introspection: https://signin.paramark.com/oauth2/introspection\n    device_authorization: https://signin.paramark.com/oauth2/device_authorization\n    registration: https://signin.paramark.com/oauth2/register\n    jwks: https://signin.paramark.com/oauth2/jwks\n  grant_types:\n  - authorization_code\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:device_code\n  response_types:\n  - code\n  response_modes:\n  - query\n  code_challenge_methods:\n  - S256\n  token_endpoint_auth_methods:\n  - none\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values:\n  - RS256\n\
  \  subject_types:\n  - public\n  scopes:\n  - openid\n  - profile\n  - email\n  - offline_access\n  dynamic_client_registration: true\n  client_id_metadata_document_supported: true\n  x-evidence:\n    fetched: '2026-08-12'\n    url: https://signin.paramark.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json; charset=utf-8\n- name: Paramark API (contract gated)\n  host: api.paramark.com\n  type: http\n  scheme: basic\n  observed: >-\n    GET https://api.paramark.com/openapi.json returns HTTP 401 with the response header\n    \"www-authenticate: Basic\" and body {\"detail\":\"Unauthorized\"}. The interactive FastAPI docs at\n    /docs and /redoc return the same 401. GET /healthz returns HTTP 200 {\"status\":\"ok\"}\n    anonymously, so the service is live; only the contract and its reference are walled.\n  runtime_auth_scheme_unknown: true\n  runtime_auth_note: >-\n    The HTTP Basic challenge guards the documentation endpoints. Paramark publishes\
  \ no reference\n    describing how a caller authenticates against the API's own operations, so the runtime scheme\n    (bearer token from the OIDC issuer above, static API key, or Basic) is NOT recorded here.\n    Determining it requires credentials we do not hold; it is not guessed.\n  x-evidence:\n    fetched: '2026-08-12'\n    url: https://api.paramark.com/openapi.json\n    http_status: 401\n    www_authenticate: Basic\n    server: uvicorn\ngaps:\n- No public authentication documentation page exists on paramark.com or any subdomain.\n- No /.well-known/oauth-protected-resource is served on the API host, so an agent cannot\n  discover which authorization server protects api.paramark.com from the resource itself.\n- No security.txt is served on any host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paramark/refs/heads/main/authentication/paramark-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Applications
- Marketing
- Analytics
- Measurement
- Marketing Mix Modeling
- Incrementality
- Advertising
- AI
---
