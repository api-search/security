---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Kleio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Kleio secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Kleio
provider_slug: kleio
scheme_count: 2
schemes:
- code_challenge_methods:
  - S256
  flows:
  - audience: https://chwai-api-5sj2xluyjq-od.a.run.app
    authorizationUrl: https://auth.kleio.ai/authorize
    flow: authorizationCode
    note: The authorization_endpoint the gateway advertises carries a pinned audience query parameter naming the Cloud Run service behind the gateway. Recorded verbatim because it is the resource indicator a token must be minted for; it is not a separately documented API host.
    tokenUrl: https://auth.kleio.ai/oauth/token
  grant_types:
  - authorization_code
  - refresh_token
  issuer: https://auth.kleio.ai/
  jwks_uri: https://auth.kleio.ai/.well-known/jwks.json
  name: KleioPlatformOAuth
  registration_endpoint: https://api.kleio.ai/api/oauth/register
  response_types:
  - code
  source: https://api.kleio.ai/.well-known/oauth-authorization-server
  type: oauth2
- code_challenge_methods:
  - S256
  - plain
  device_authorization_endpoint: https://auth.kleio.ai/oauth/device/code
  issuer: https://auth.kleio.ai/
  name: KleioOIDC
  openIdConnectUrl: https://auth.kleio.ai/.well-known/openid-configuration
  registration_endpoint: https://auth.kleio.ai/oidc/register
  response_modes:
  - query
  - fragment
  - form_post
  revocation_endpoint: https://auth.kleio.ai/oauth/revoke
  source: https://auth.kleio.ai/.well-known/openid-configuration
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - none
  token_endpoint_auth_signing_algs:
  - RS256
  - RS384
  - PS256
  type: openIdConnect
  userinfo_endpoint: https://auth.kleio.ai/userinfo
slug: kleio-authentication
source_filename: kleio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: probed\nsource: https://api.kleio.ai/.well-known/oauth-authorization-server\nalso_source: https://auth.kleio.ai/.well-known/openid-configuration\nnote: 'Derived from the two machine-readable discovery documents Kleio actually serves, not from an\n  OpenAPI — Kleio publishes no specification and no public authentication documentation. The scripted\n  derive (derive-authentication.py) found zero schemes because there is no spec in the repo to read; this\n  profile is written from the probed RFC 8414 and OpenID Connect discovery documents saved verbatim under\n  well-known/. Everything below is a value Kleio published; nothing is inferred about operation-level\n  security, which is not observable without credentials.'\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  pkce: required\n  pkce_methods:\n  - S256\n  dynamic_client_registration: true\n  identity_provider: Auth0 (EU tenant)\n\
  schemes:\n- name: KleioPlatformOAuth\n  type: oauth2\n  source: https://api.kleio.ai/.well-known/oauth-authorization-server\n  issuer: https://auth.kleio.ai/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://auth.kleio.ai/authorize\n    tokenUrl: https://auth.kleio.ai/oauth/token\n    audience: https://chwai-api-5sj2xluyjq-od.a.run.app\n    note: 'The authorization_endpoint the gateway advertises carries a pinned audience query parameter\n      naming the Cloud Run service behind the gateway. Recorded verbatim because it is the resource\n      indicator a token must be minted for; it is not a separately documented API host.'\n  grant_types:\n  - authorization_code\n  - refresh_token\n  response_types:\n  - code\n  code_challenge_methods:\n  - S256\n  registration_endpoint: https://api.kleio.ai/api/oauth/register\n  jwks_uri: https://auth.kleio.ai/.well-known/jwks.json\n- name: KleioOIDC\n  type: openIdConnect\n  source: https://auth.kleio.ai/.well-known/openid-configuration\n\
  \  openIdConnectUrl: https://auth.kleio.ai/.well-known/openid-configuration\n  issuer: https://auth.kleio.ai/\n  userinfo_endpoint: https://auth.kleio.ai/userinfo\n  revocation_endpoint: https://auth.kleio.ai/oauth/revoke\n  device_authorization_endpoint: https://auth.kleio.ai/oauth/device/code\n  registration_endpoint: https://auth.kleio.ai/oidc/register\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  token_endpoint_auth_signing_algs:\n  - RS256\n  - RS384\n  - PS256\n  code_challenge_methods:\n  - S256\n  - plain\n  response_modes:\n  - query\n  - fragment\n  - form_post\n  subject_types:\n  - public\nobservations:\n- 'Dynamic client registration is open on the gateway itself (api.kleio.ai/api/oauth/register returns 405\n  to GET, confirming the route is defined and expects POST). Open DCR plus authorization-code with S256\n  PKCE is the exact shape the MCP authorization specification prescribes, which is consistent with\
  \ the\n  MCP/UCP integration Kleio markets — but no MCP endpoint is published, so the pairing cannot be\n  confirmed from outside.'\n- 'The gateway rejects every undefined path with a Google Cloud API Gateway 404 (\"The current request is\n  not defined by this API\"), so the route table is closed and cannot be enumerated anonymously.'\n- 'No API-key scheme was observed anywhere. There is no public auth guide, quickstart, or token page.'\ngaps:\n- 'No published authentication documentation on kleio.ai — the only auth contract a developer can read is\n  the discovery metadata captured here.'\n- 'No /.well-known/oauth-protected-resource (RFC 9728) on api.kleio.ai, so resource-server metadata is\n  not discoverable.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kleio/refs/heads/main/authentication/kleio-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Company
- Ai Data
- Agentic Commerce
- AI Agents
- Enterprise Sales
- Conversational AI
- Knowledge Engine
- Model Context Protocol
- Agent To Agent
- Retail
- Travel
- Real Estate
- Automotive
- France
---
