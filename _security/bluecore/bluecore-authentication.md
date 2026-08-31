---
api_key_in:
- header
api_specs:
- filename: bluecore-authn-api-openapi.yml
  format: yaml
  label: Bluecore Authn API
  slug: bluecore-authn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-authn-api-openapi.yml
- filename: bluecore-campaignsapipublic-api-openapi.yml
  format: yaml
  label: Bluecore CampaignsAPIPublic API
  slug: bluecore-campaignsapipublic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-campaignsapipublic-api-openapi.yml
- filename: bluecore-direct-send-api-openapi.yml
  format: yaml
  label: Bluecore Direct send API
  slug: bluecore-direct-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-direct-send-api-openapi.yml
- filename: bluecore-eligibility-api-openapi.yml
  format: yaml
  label: Bluecore Eligibility API
  slug: bluecore-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-eligibility-api-openapi.yml
- filename: bluecore-profile-api-openapi.yml
  format: yaml
  label: Bluecore Profile API
  slug: bluecore-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-profile-api-openapi.yml
- filename: bluecore-transactional-api-openapi.yml
  format: yaml
  label: Bluecore Transactional API
  slug: bluecore-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-transactional-api-openapi.yml
- filename: bluecore-get-status-api-openapi.yml
  format: yaml
  label: Bluecore GET STATUS API
  slug: bluecore-get-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-get-status-api-openapi.yml
- filename: bluecore-send-email-api-openapi.yml
  format: yaml
  label: Bluecore SEND EMAIL API
  slug: bluecore-send-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-send-email-api-openapi.yml
auth_types:
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Bluecore Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bluecore secures its APIs with oauth2 and http-bearer across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bluecore
provider_slug: bluecore
scheme_count: 3
schemes:
- description: Bearer access token obtained from the client-credentials token endpoint. Value is "Bearer " followed by the token returned by POST https://auth.bluecore.com/oauth/token.
  in: header
  name: GlooAuth
  parameter: authorization
  scheme: bearer
  sources:
  - openapi/bluecore-openapi.yml
  - https://developers.bluecore.com/reference/authn_getaccesstoken
  type: http
- applies_to: https://api.bluecore.com/email/
  description: 'The LEGACY transactional API is protected by a long-lived, customer-specific API key issued by Bluecore, sent as `Authorization: Bearer {Bluecore API Key}`. There is no token endpoint, no expiry, no scopes and no rotation flow documented; the published contract says to email support@bluecore.com to obtain or cycle a key, and warns the key must never be used from a browser. This is a materially weaker auth model than the OAuth surface and is on a different host — an integrator on the legacy API gains nothing from the OAuth documentation.'
  in: header
  name: TransactionalStaticKey
  parameter: Authorization
  scheme: bearer
  sources:
  - openapi/bluecore-transactional-legacy-api-openapi.yml
  - https://www.bluecore.com/transactional-api-docs/
  type: http
- applies_to: https://api.bluecore.app/api/track/mobile/v1
  description: The Events API authenticates with the tenant `token` (the Bluecore namespace) carried inside the JSON request body rather than in a header. No Authorization header, no expiry, no scopes. Because the same token is embedded in the client-side website tag, it is a public write credential by design.
  in: body
  name: EventsTenantToken
  parameter: properties.token
  sources:
  - https://help.bluecore.com/help/events-api
  type: apiKey
slug: bluecore-authentication
source_filename: bluecore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.bluecore.com/reference/authn\ndocs: https://developers.bluecore.com/reference/authn\nsummary:\n  model: oauth2-client-credentials\n  types:\n  - oauth2\n  - http-bearer\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Bluecore uses the standard OAuth 2.0 client-credentials grant. Clients POST client_id +\n    client_secret to https://auth.bluecore.com/oauth/token (audience https://a.bluecore.com,\n    grant_type client_credentials) and receive a Bearer access_token valid for 24 hours (86,400s).\n    Requests to the API then send `authorization: Bearer <token>`. In the published per-operation\n    OpenAPI the bearer scheme is modelled as an apiKey security scheme named \"GlooAuth\"\n    (in: header, name: authorization) rather than an oauth2 scheme, so the mechanical oauth2\n    scope derivation does not fire; the real flow and scopes are captured here and in scopes/.\n\
  schemes:\n- name: GlooAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: authorization\n  description: >-\n    Bearer access token obtained from the client-credentials token endpoint. Value is\n    \"Bearer \" followed by the token returned by POST https://auth.bluecore.com/oauth/token.\n  sources:\n  - openapi/bluecore-openapi.yml\n  - https://developers.bluecore.com/reference/authn_getaccesstoken\n- name: TransactionalStaticKey\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  applies_to: https://api.bluecore.com/email/\n  description: >-\n    The LEGACY transactional API is protected by a long-lived, customer-specific API key issued by\n    Bluecore, sent as `Authorization: Bearer {Bluecore API Key}`. There is no token endpoint, no\n    expiry, no scopes and no rotation flow documented; the published contract says to email\n    support@bluecore.com to obtain or cycle a key, and warns the key must never be used from a\n    browser. This is a materially\
  \ weaker auth model than the OAuth surface and is on a different\n    host — an integrator on the legacy API gains nothing from the OAuth documentation.\n  sources:\n  - openapi/bluecore-transactional-legacy-api-openapi.yml\n  - https://www.bluecore.com/transactional-api-docs/\n- name: EventsTenantToken\n  type: apiKey\n  in: body\n  parameter: properties.token\n  applies_to: https://api.bluecore.app/api/track/mobile/v1\n  description: >-\n    The Events API authenticates with the tenant `token` (the Bluecore namespace) carried inside\n    the JSON request body rather than in a header. No Authorization header, no expiry, no scopes.\n    Because the same token is embedded in the client-side website tag, it is a public write\n    credential by design.\n  sources:\n  - https://help.bluecore.com/help/events-api\ntoken_endpoint:\n  url: https://auth.bluecore.com/oauth/token\n  grant_type: client_credentials\n  audience: https://a.bluecore.com\n  token_type: Bearer\n  expires_in: 86400\n  credentials_docs:\
  \ https://help.bluecore.com/help/create-an-api-key\nauthorization_server:\n  generated: '2026-08-13'\n  method: probed\n  issuer: https://auth.bluecore.com/\n  platform: Auth0\n  discovery:\n  - {path: /.well-known/oauth-authorization-server, status: 200, spec: RFC 8414,\n     file: well-known/bluecore-oauth-authorization-server.json}\n  - {path: /.well-known/openid-configuration, status: 200, spec: 'OpenID Connect Discovery 1.0',\n     file: well-known/bluecore-openid-configuration.json}\n  - {path: /.well-known/jwks.json, status: 200, spec: RFC 7517, file: well-known/bluecore-jwks.json}\n  endpoints:\n    authorization: https://auth.bluecore.com/authorize\n    token: https://auth.bluecore.com/oauth/token\n    device_authorization: https://auth.bluecore.com/oauth/device/code\n    userinfo: https://auth.bluecore.com/userinfo\n    revocation: https://auth.bluecore.com/oauth/revoke\n    registration: https://auth.bluecore.com/oidc/register\n    jwks: https://auth.bluecore.com/.well-known/jwks.json\n\
  \  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, private_key_jwt, none]\n  code_challenge_methods_supported: [S256, plain]\n  signing_algs: [RS256, RS384, PS256]\n  detail: >-\n    Discovered 2026-08-13 — round 1 recorded \"no /.well-known/ documents on any Bluecore host\"\n    because auth.bluecore.com had not been probed. The metadata describes the authorization server\n    that actually issues Bluecore API access tokens, so a client can now discover the token\n    endpoint and verify token signatures without reading the docs. Note the advertised scope set\n    (openid, profile, email, phone, address, offline_access) is the generic Auth0 OIDC set and is\n    NOT the Bluecore API scope vocabulary — the real API scopes are the `resource:verb` strings in\n    scopes/bluecore-scopes.yml.\nmulti_surface_warning: >-\n  Bluecore operates three API surfaces with three different and incompatible auth models:\n  OAuth 2.0 client-credentials (a.bluecore.com/api),\
  \ a static Bearer API key\n  (api.bluecore.com/email/, legacy), and a tenant token inside the request body\n  (api.bluecore.app/api/track/mobile/v1). See conventions/bluecore-conventions.yml\n  surface_divergence.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/authentication/bluecore-authentication.yml
summary_line: oauth2/http-bearer · 3 schemes
tags:
- Company
- Retail
- Marketing
- Customer Data Platform
- Personalization
- Email
- SMS
- Messaging
- E-Commerce
- Consent
---
