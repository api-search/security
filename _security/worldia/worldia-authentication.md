---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication profile for the Worldia production API, established by probing https://api.worldia.com anonymously on 2026-09-04. Worldia publishes no authentication documentation, no developer portal and no self-service signup, so this profile is read from live challenge responses rather than from a docs page.
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Worldia Authentication
name_suffix: Authentication
oauth_flows: []
overview: Worldia declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Worldia
provider_slug: worldia
scheme_count: 2
schemes:
- bearer_format: JWT
  evidence:
    http_status: 401
    response_body: '{"code":401,"message":"JWT Token not found"}'
    response_header: 'www-authenticate: Bearer'
    url: https://api.worldia.com/customers
  header: Authorization
  id: bearerJwt
  implementation: The challenge string "JWT Token not found" is the default message of LexikJWTAuthenticationBundle, the Symfony JWT bundle that Worldia forks publicly in its own GitHub organization (github.com/worldia/LexikJWTAuthenticationBundle, alongside github.com/worldia/JWTRefreshTokenBundle). The refresh-token fork indicates a refresh-token flow exists behind the wall, though no refresh endpoint is publicly routed.
  in: header
  scheme: bearer
  token_endpoint: unknown
  token_endpoint_note: No token endpoint is publicly routed under the conventional names. POST to /authentication_token, /login_check, /api/login_check, /token, /oauth/token and /refresh_token all return 404. POST /login returns 400 rather than 404, so a route exists at that path, but no request shape is documented and none was guessed.
  type: http
- evidence:
    detail: You must set the "X-Channel" header to a registered channel.
    http_status: 400
    url: https://api.worldia.com/inspirations
  header: X-Channel
  id: channelHeader
  in: header
  is_credential: false
  note: 'X-Channel is a required tenant discriminator, not a secret. It is explicitly NOT a credential: the complete set of 388 valid channel codes is readable anonymously at GET /channels, and supplying one grants access to the public catalogue surface without any token. It is recorded here because a caller cannot reach channel-scoped collections without it, so it belongs in any integration''s request-signing path even though it carries no authorization weight.'
  role: tenant-selector
  type: apiKey
slug: worldia-authentication
source_filename: worldia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: https://api.worldia.com/customers\nname: Worldia API Authentication\ndescription: >-\n  Authentication profile for the Worldia production API, established by probing\n  https://api.worldia.com anonymously on 2026-09-04. Worldia publishes no authentication\n  documentation, no developer portal and no self-service signup, so this profile is read\n  from live challenge responses rather than from a docs page.\ndocs: null\n\nschemes:\n  - id: bearerJwt\n    type: http\n    scheme: bearer\n    bearer_format: JWT\n    in: header\n    header: Authorization\n    evidence:\n      url: https://api.worldia.com/customers\n      http_status: 401\n      response_header: 'www-authenticate: Bearer'\n      response_body: '{\"code\":401,\"message\":\"JWT Token not found\"}'\n    implementation: >-\n      The challenge string \"JWT Token not found\" is the default message of\n      LexikJWTAuthenticationBundle, the Symfony JWT bundle that Worldia\
  \ forks publicly in its\n      own GitHub organization (github.com/worldia/LexikJWTAuthenticationBundle, alongside\n      github.com/worldia/JWTRefreshTokenBundle). The refresh-token fork indicates a\n      refresh-token flow exists behind the wall, though no refresh endpoint is publicly\n      routed.\n    token_endpoint: unknown\n    token_endpoint_note: >-\n      No token endpoint is publicly routed under the conventional names. POST to\n      /authentication_token, /login_check, /api/login_check, /token, /oauth/token and\n      /refresh_token all return 404. POST /login returns 400 rather than 404, so a route\n      exists at that path, but no request shape is documented and none was guessed.\n\n  - id: channelHeader\n    type: apiKey\n    in: header\n    header: X-Channel\n    role: tenant-selector\n    is_credential: false\n    evidence:\n      url: https://api.worldia.com/inspirations\n      http_status: 400\n      detail: 'You must set the \"X-Channel\" header to a registered channel.'\n\
  \    note: >-\n      X-Channel is a required tenant discriminator, not a secret. It is explicitly NOT a\n      credential: the complete set of 388 valid channel codes is readable anonymously at\n      GET /channels, and supplying one grants access to the public catalogue surface without\n      any token. It is recorded here because a caller cannot reach channel-scoped\n      collections without it, so it belongs in any integration's request-signing path even\n      though it carries no authorization weight.\n\noauth2:\n  supported: false\n  evidence: >-\n    /.well-known/openid-configuration and /.well-known/oauth-authorization-server return 404\n    on every Worldia host probed (worldia.com, www, corp, api, content, careers,\n    experts-usa, static). No OAuth flow, authorization server or scope surface is published.\nscopes:\n  published: false\n  artifact: null\n  note: >-\n    scopes/ is deliberately not written. The API is bearer-JWT authenticated with no OAuth2\n    securityScheme\
  \ and no published permission reference, so there is no scope surface to\n    record; an empty scopes artifact would assert a structure Worldia does not have.\n\nmtls:\n  supported: unknown\nopenid_connect:\n  supported: false\n\nanonymous_surface:\n  description: >-\n    An unusually large read surface is reachable with no credential at all, which is worth\n    recording because it is the only part of this API a third party can actually evaluate.\n  collections:\n    - path: /channels\n      http_status: 200\n      total_items: 388\n      requires_channel_header: false\n    - path: /locations\n      http_status: 200\n      requires_channel_header: false\n      note: 'Verified via GET /locations?type=continent&promoted=true (10 items).'\n    - path: /themes\n      http_status: 200\n      total_items: 24\n      requires_channel_header: true\n    - path: /accommodations\n      http_status: 200\n      total_items: 16943\n      requires_channel_header: true\n    - path: /inspirations\n   \
  \   http_status: 200\n      total_items: 971\n      requires_channel_header: true\n    - path: /airports\n      http_status: 200\n      total_items: 0\n      requires_channel_header: true\n    - path: /contexts/{Type}\n      http_status: 200\n      requires_channel_header: false\n      note: 'JSON-LD context documents; see json-ld/worldia-json-ld.yml.'\n  authenticated_only:\n    - path: /customers\n      http_status: 401\n      challenge: 'www-authenticate: Bearer'\n    - path: /templates\n      http_status: 403\n      detail: 'Unable to access as unauthorized user'\n  inconsistency_note: >-\n    /customers rejects anonymous callers with 401 while /templates rejects them with 403.\n    Both are anonymous requests, so both should be 401 under RFC 9110; a client cannot rely\n    on the status code to decide whether to acquire a token or to give up.\n\naccess_model:\n  self_service: false\n  note: >-\n    There is no signup, no key issuance page and no sandbox. Access is obtained through\
  \ a\n    commercial partnership — the only conversion path on corp.worldia.com is a HubSpot\n    \"Book a demo\" form. See plans/worldia-plans-pricing.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldia/refs/heads/main/authentication/worldia-authentication.yml
summary_line: 2 schemes
tags:
- Travel
- Tourism
- Booking
- Trip Planning
- Travel Technology
- Hospitality
- B2B2C
- White Label
- Itinerary
- Distribution
---
