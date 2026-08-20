---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: probed
name: Avarra Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Avarra secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Avarra
provider_slug: avarra
scheme_count: 1
schemes:
- authorization_endpoint: null
  flows:
  - flow: clientCredentials
    note: The authorization server metadata declares no scopes_supported and the token endpoint is not anonymously enumerable, so no scope vocabulary is published. No scopes/ artifact is emitted for this provider.
    scopes: {}
    tokenUrl: https://api.avarra.ai/oauth/token
  introspection_endpoint: https://api.avarra.ai/oauth/introspect
  issuer: https://api.avarra.ai
  jwks_uri: https://api.avarra.ai/.well-known/jwks.json
  name: oauth2ClientCredentials
  response_types_supported: []
  sources:
  - well-known/avarra-oauth-authorization-server.json
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  type: oauth2
slug: avarra-authentication
source_filename: avarra-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: probed\nsource: https://api.avarra.ai/.well-known/oauth-authorization-server\nnote: >-\n  Avarra publishes no OpenAPI and no developer documentation, so this profile is read\n  directly off the RFC 8414 Authorization Server Metadata document the API host serves\n  anonymously, plus the live error envelopes returned by the token, introspection and\n  /v1 resource endpoints. Every field below was observed on the wire on 2026-08-14 -\n  none of it is inferred from marketing copy.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  public_docs: false\n  discovery: RFC 8414 authorization server metadata\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  sources:\n  - well-known/avarra-oauth-authorization-server.json\n  issuer: https://api.avarra.ai\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.avarra.ai/oauth/token\n    scopes: {}\n    note: >-\n      The authorization server\
  \ metadata declares no scopes_supported and the token\n      endpoint is not anonymously enumerable, so no scope vocabulary is published.\n      No scopes/ artifact is emitted for this provider.\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  introspection_endpoint: https://api.avarra.ai/oauth/introspect\n  jwks_uri: https://api.avarra.ai/.well-known/jwks.json\n  response_types_supported: []\n  authorization_endpoint: null\nresource_server:\n  base: https://api.avarra.ai\n  version_prefix: /v1\n  bearer_header: Authorization\n  unauthenticated_status: 401\n  unauthenticated_body: '{\"error\":\"unauthorized\",\"message\":\"missing or invalid authorization\n    header\"}'\n  www_authenticate_header: false\n  note: >-\n    The resource server returns a 401 with a JSON envelope but does NOT emit a\n    WWW-Authenticate challenge header, so an RFC 6750 client cannot discover the\n    realm or the required scope from the response. There is also no\n    /.well-known/oauth-protected-resource\
  \ (RFC 9728) document, so the resource\n    server does not advertise its authorization server. Both are gaps a client has\n    to be told about out of band.\njwks:\n  url: https://api.avarra.ai/.well-known/jwks.json\n  file: well-known/avarra-jwks.json\n  keys: 1\n  kty: RSA\n  kid: 5d22a766-d768-41e0-bbfc-ac0aa04afe90\n  alg_declared: false\n  use_declared: false\n  note: >-\n    Public signing key set - published deliberately for token verification. The key\n    entry omits \"alg\" and \"use\", which RFC 7517 makes optional but which verifiers\n    normally rely on.\nobserved:\n- request: GET https://api.avarra.ai/.well-known/oauth-authorization-server\n  status: 200\n- request: GET https://api.avarra.ai/.well-known/jwks.json\n  status: 200\n- request: POST https://api.avarra.ai/oauth/token (grant_type=client_credentials, no\n    credentials)\n  status: 401\n  body: '{\"error\":\"invalid_request\",\"error_description\":\"missing client credentials\"}'\n- request: POST https://api.avarra.ai/oauth/introspect\
  \ (no credentials)\n  status: 401\n  body: '{\"error\":\"invalid_request\",\"error_description\":\"missing client credentials\"}'\n- request: GET https://api.avarra.ai/oauth/authorize\n  status: 404\n- request: GET https://api.avarra.ai/v1/me\n  status: 401\ndocs: null\ndocs_note: >-\n  Avarra publishes no authentication documentation. /docs, /developers, /api and\n  /integrations on www.avarra.ai all return 404. Credentials are presumably issued\n  through the commercial relationship (request-a-demo).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avarra/refs/heads/main/authentication/avarra-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Sales Enablement
- Sales Training
- Artificial Intelligence
- Coaching
- Role-Play Simulation
- Revenue Operations
- Onboarding
- Sales Readiness
- Conversation Intelligence
---
