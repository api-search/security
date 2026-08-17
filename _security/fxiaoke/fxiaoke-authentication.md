---
api_key_in:
- header
- body
auth_types:
- oauth2
- custom-token
description: ''
kind: authentication
layout: security
method: searched
name: Fxiaoke Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Fxiaoke secures its APIs with oauth2 and custom-token across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Fxiaoke
provider_slug: fxiaoke
scheme_count: 4
schemes:
- caching_guidance: 'Calling within the first 6600s returns the SAME token; calling between 6600s and 7200s issues a NEW token while the old one stays valid until 7200s. The documented contract is therefore: cache for 6600s, refresh in the 6600–7200s window, and key retry logic off errorCode 20016.'
  description: 客户端凭证模式. A tenant creates a self-built app in the Fxiaoke admin console with developer mode enabled and receives appId, appSecret and permanentCode. These are exchanged for a short-lived corpAccessToken that authenticates all subsequent Open API v2 calls. The mode supports acting as any employee by supplying their ID.
  documented: true
  endpoint_limits:
    concurrency: not permitted (不能并发调用本接口)
    rate: 10 calls per minute
  flow: clientCredentials
  name: enterprise-app-token
  ref: rate-limits/fxiaoke-rate-limits.yml
  request:
    content_type: application/json
    fields:
    - name: appId
      required: true
    - name: appSecret
      required: true
    - name: permanentCode
      required: true
    - name: grantType
      required: true
      value: app_secret
    headers: none — the token call is the one endpoint that sends no auth headers
    method: POST
  response_fields:
  - accessToken
  - expiresIn
  - openUserId
  - appId
  - ea
  - errorCode
  - errorMessage
  - traceId
  token_endpoint: https://open.fxiaoke.com/oauth2.0/token
  token_endpoint_legacy: https://open.fxiaoke.com/cgi/corpAccessToken/get/V2
  token_lifetime_seconds: 7200
  token_query_params:
  - thirdTraceId
  type: oauth2
- access_token_lifetime_seconds: 7200
  authorization_endpoint: https://open.fxiaoke.com/oauth2.0/authorize
  authorize_params:
  - name: appId
    required: true
    standard_name: client_id
  - name: redirectUrl
    required: true
    standard_name: redirect_uri
  - name: responseType
    required: true
    standard_name: response_type
    value: code
  - name: state
    required: true
  - name: thirdTraceId
    required: true
    standard_name: null
  csrf: state is mandatory and the docs require the app to verify it on callback, with a recommended construction of MD5(timestamp + account).
  description: 授权码模式, for web applications with a backend that need to act as an end user. The user is redirected to Fxiaoke, authorizes, and the app exchanges the returned code for an access token plus a refresh token.
  documented: true
  flow: authorizationCode
  name: authorization-code
  pkce: false
  redirect_uri_binding: The redirectUrl domain must match the login-authorization domain registered on the app detail page.
  refresh_token_lifetime: 2 months
  response_fields:
  - openUserId
  - accessToken
  - corpId
  - expiresIn
  - refreshToken
  - errorCode
  - errorMessage
  spec_deviation: Parameter names are camelCase Fxiaoke names, not RFC 6749 names — appId not client_id, redirectUrl not redirect_uri, responseType not response_type, grantType not grant_type. A standards-compliant OAuth client library cannot drive this flow without custom parameter mapping. The token exchange also sends appSecret in a JSON body rather than using a documented client authentication method.
  token_endpoint: https://open.fxiaoke.com/oauth2.0/token
  token_params:
  - name: appId
    required: true
  - name: appSecret
    required: true
  - name: redirectUrl
    required: true
  - name: code
    required: true
  - name: grantType
    required: true
    value: authorization_code
  type: oauth2
- authorization_endpoint: https://open.fxiaoke.com/oauth2.0/cli/authorize
  caveats:
  - jwks_uri returns an empty key set ({"keys":[]}) as of 2026-08-13, so an RS256 id_token cannot be verified by any client following discovery.
  - No matching RFC 9728 oauth-protected-resource metadata is served — the path returns the gateway's errorCode 10006 envelope — so there is no advertised resource server for these tokens.
  - No scopes_supported is advertised and no scope registry is published anywhere.
  code_challenge_methods:
  - S256
  description: An RFC 8414-conformant authorization server advertised at https://open.fxiaoke.com/.well-known/oauth-authorization-server but absent from the developer manual. Public clients (token_endpoint_auth_methods_supported ["none"]) use PKCE S256 with authorization_code and refresh_token grants and may self-register through the RFC 7591 dynamic client registration endpoint. The "cli" and "pkce" path segments and the anonymous-client posture are the shape a CLI or agent client expects.
  documented: false
  evidence: well-known/fxiaoke-oauth-authorization-server.json
  flow: authorizationCode
  grant_types:
  - authorization_code
  - refresh_token
  id_token_signing_alg:
  - RS256
  issuer: https://open.fxiaoke.com/oauth2.0
  jwks_uri: https://open.fxiaoke.com/oauth2.0/jwks
  name: oauth2.1-pkce
  probed: '2026-08-13'
  registration_endpoint: https://open.fxiaoke.com/oauth2.0/register
  response_types:
  - code
  scopes_supported: null
  subject_types:
  - public
  token_endpoint: https://open.fxiaoke.com/oauth2.0/pkce/token
  token_endpoint_auth_methods:
  - none
  type: oauth2
- description: Client-side JS API calls are authorized by a sha1 signature rather than a bearer token. A jsapi_ticket (7200s lifetime) is fetched server-side with the corpAccessToken, then signed together with a nonce, timestamp and the page URL.
  documented: true
  name: jsapi-ticket-signature
  ref: components/fxiaoke-components.yml
  signature_algorithm: sha1 of the ASCII-sorted key=value string built from noncestr, jsapi_ticket, timestamp and url (fragment removed); result uppercased hex.
  ticket_endpoint: https://open.fxiaoke.com/cgi/jsApiTicket/get
  ticket_request_fields:
  - corpAccessToken
  - corpId
  ticket_response_fields:
  - ticket
  - expiresIn
  - errorCode
  - errorMessage
  type: custom-signature
slug: fxiaoke-authentication
source_filename: fxiaoke-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://developer.fxiaoke.com/openapi_v2/start/auth/app-info.html\ndocs:\n- https://developer.fxiaoke.com/openapi_v2/start/auth/app-info.html\n- https://developer.fxiaoke.com/openapi_v2/start/auth/auth-code.html\n- https://developer.fxiaoke.com/openapi_v2/start/auth/refresh.html\n- https://developer.fxiaoke.com/openapi_v2/start/example/public.html\n- https://developer.fxiaoke.com/openapi_v2/start/example/old.html\n- https://open.fxiaoke.com/.well-known/oauth-authorization-server\nsummary:\n  types: [oauth2, custom-token]\n  api_key_in: [header, body]\n  oauth2_flows: [clientCredentials, authorizationCode]\n  base_host: https://open.fxiaoke.com\n  surfaces: 2\n  note: >-\n    Fxiaoke runs TWO distinct OAuth surfaces that do not share endpoints or parameter\n    names — the documented developer flow under /oauth2.0/{authorize,token}, and an\n    undocumented RFC 8414-conformant PKCE server whose metadata advertises\n    /oauth2.0/cli/authorize\
  \ and /oauth2.0/pkce/token. Only the first is described in the\n    developer manual.\n\nschemes:\n- name: enterprise-app-token\n  type: oauth2\n  flow: clientCredentials\n  documented: true\n  description: >-\n    客户端凭证模式. A tenant creates a self-built app in the Fxiaoke admin console with\n    developer mode enabled and receives appId, appSecret and permanentCode. These are\n    exchanged for a short-lived corpAccessToken that authenticates all subsequent Open\n    API v2 calls. The mode supports acting as any employee by supplying their ID.\n  token_endpoint: https://open.fxiaoke.com/oauth2.0/token\n  token_endpoint_legacy: https://open.fxiaoke.com/cgi/corpAccessToken/get/V2\n  token_query_params:\n  - thirdTraceId   # caller-supplied UUIDv4, required, must be unique per request\n  request:\n    content_type: application/json\n    method: POST\n    headers: none — the token call is the one endpoint that sends no auth headers\n    fields:\n    - {name: appId, required: true}\n    - {name:\
  \ appSecret, required: true}\n    - {name: permanentCode, required: true}\n    - {name: grantType, required: true, value: app_secret}\n  response_fields:\n  - accessToken\n  - expiresIn\n  - openUserId    # carries the enterprise openCorpId in this flow\n  - appId\n  - ea            # enterprise account, becomes the x-fs-ea header\n  - errorCode\n  - errorMessage\n  - traceId\n  token_lifetime_seconds: 7200\n  caching_guidance: >-\n    Calling within the first 6600s returns the SAME token; calling between 6600s and\n    7200s issues a NEW token while the old one stays valid until 7200s. The documented\n    contract is therefore: cache for 6600s, refresh in the 6600–7200s window, and key\n    retry logic off errorCode 20016.\n  endpoint_limits:\n    rate: 10 calls per minute\n    concurrency: not permitted (不能并发调用本接口)\n  ref: rate-limits/fxiaoke-rate-limits.yml\n\n- name: authorization-code\n  type: oauth2\n  flow: authorizationCode\n  documented: true\n  description: >-\n    授权码模式, for\
  \ web applications with a backend that need to act as an end user. The\n    user is redirected to Fxiaoke, authorizes, and the app exchanges the returned code\n    for an access token plus a refresh token.\n  authorization_endpoint: https://open.fxiaoke.com/oauth2.0/authorize\n  token_endpoint: https://open.fxiaoke.com/oauth2.0/token\n  authorize_params:\n  - {name: appId, required: true, standard_name: client_id}\n  - {name: redirectUrl, required: true, standard_name: redirect_uri}\n  - {name: responseType, required: true, value: code, standard_name: response_type}\n  - {name: state, required: true}\n  - {name: thirdTraceId, required: true, standard_name: null}\n  token_params:\n  - {name: appId, required: true}\n  - {name: appSecret, required: true}\n  - {name: redirectUrl, required: true}\n  - {name: code, required: true}\n  - {name: grantType, required: true, value: authorization_code}\n  response_fields: [openUserId, accessToken, corpId, expiresIn, refreshToken, errorCode, errorMessage]\n\
  \  access_token_lifetime_seconds: 7200\n  refresh_token_lifetime: 2 months\n  pkce: false\n  csrf: >-\n    state is mandatory and the docs require the app to verify it on callback, with a\n    recommended construction of MD5(timestamp + account).\n  redirect_uri_binding: >-\n    The redirectUrl domain must match the login-authorization domain registered on the\n    app detail page.\n  spec_deviation: >-\n    Parameter names are camelCase Fxiaoke names, not RFC 6749 names — appId not\n    client_id, redirectUrl not redirect_uri, responseType not response_type, grantType\n    not grant_type. A standards-compliant OAuth client library cannot drive this flow\n    without custom parameter mapping. The token exchange also sends appSecret in a JSON\n    body rather than using a documented client authentication method.\n\n- name: oauth2.1-pkce\n  type: oauth2\n  flow: authorizationCode\n  documented: false\n  description: >-\n    An RFC 8414-conformant authorization server advertised at\n    https://open.fxiaoke.com/.well-known/oauth-authorization-server\
  \ but absent from the\n    developer manual. Public clients (token_endpoint_auth_methods_supported [\"none\"])\n    use PKCE S256 with authorization_code and refresh_token grants and may self-register\n    through the RFC 7591 dynamic client registration endpoint. The \"cli\" and \"pkce\" path\n    segments and the anonymous-client posture are the shape a CLI or agent client\n    expects.\n  issuer: https://open.fxiaoke.com/oauth2.0\n  authorization_endpoint: https://open.fxiaoke.com/oauth2.0/cli/authorize\n  token_endpoint: https://open.fxiaoke.com/oauth2.0/pkce/token\n  registration_endpoint: https://open.fxiaoke.com/oauth2.0/register\n  jwks_uri: https://open.fxiaoke.com/oauth2.0/jwks\n  grant_types: [authorization_code, refresh_token]\n  response_types: [code]\n  code_challenge_methods: [S256]\n  token_endpoint_auth_methods: [none]\n  subject_types: [public]\n  id_token_signing_alg: [RS256]\n  scopes_supported: null\n  caveats:\n  - >-\n    jwks_uri returns an empty key set ({\"keys\"\
  :[]}) as of 2026-08-13, so an RS256\n    id_token cannot be verified by any client following discovery.\n  - >-\n    No matching RFC 9728 oauth-protected-resource metadata is served — the path returns\n    the gateway's errorCode 10006 envelope — so there is no advertised resource server\n    for these tokens.\n  - No scopes_supported is advertised and no scope registry is published anywhere.\n  probed: '2026-08-13'\n  evidence: well-known/fxiaoke-oauth-authorization-server.json\n\n- name: jsapi-ticket-signature\n  type: custom-signature\n  documented: true\n  description: >-\n    Client-side JS API calls are authorized by a sha1 signature rather than a bearer\n    token. A jsapi_ticket (7200s lifetime) is fetched server-side with the\n    corpAccessToken, then signed together with a nonce, timestamp and the page URL.\n  ticket_endpoint: https://open.fxiaoke.com/cgi/jsApiTicket/get\n  ticket_request_fields: [corpAccessToken, corpId]\n  ticket_response_fields: [ticket, expiresIn, errorCode,\
  \ errorMessage]\n  signature_algorithm: >-\n    sha1 of the ASCII-sorted key=value string built from noncestr, jsapi_ticket,\n    timestamp and url (fragment removed); result uppercased hex.\n  ref: components/fxiaoke-components.yml\n\ntoken_transport:\n  current:\n    style: header\n    headers:\n    - {name: authorization, value: 'Bearer <token>'}\n    - {name: x-fs-ea, value: enterprise account from the token response}\n    - {name: x-fs-userid, value: acting employee CRM ID}\n    source: https://developer.fxiaoke.com/openapi_v2/start/example/public.html\n  legacy:\n    style: body\n    fields: [corpAccessToken, currentOpenUserId, corpId]\n    source: https://developer.fxiaoke.com/openapi_v2/start/example/old.html\n    note: Still documented and functional; no sunset date published.\n\nmulti_tenancy:\n  tenant_identifier: corpId (FSCID_*) / ea\n  actor_identifier: openUserId, or x-fs-userid under the current convention\n  app_identifier: appId (FSAID_*)\n  authorization_model: >-\n\
  \    Per-app, per-enterprise grants administered by the tenant. Denials surface as\n    errorCode 15003, 20014, 20020, 20021, 20022 and 20023 rather than HTTP 403.\n\nscopes:\n  published: false\n  note: >-\n    A scope parameter exists (errorCodes 10006 and 11006 reference it) but no scope\n    values, permission catalog or consent screen inventory is published, and the RFC\n    8414 metadata omits scopes_supported. See scopes/fxiaoke-scopes.yml.\n\nnotes: >-\n  No OpenAPI/Swagger definition is published, so this profile was captured from the\n  developer documentation and live RFC 8414 metadata rather than derived from a spec.\n  The strongest auth signal is clarity: two documented grant types with complete\n  parameter tables, explicit token lifetimes and explicit caching guidance. The\n  weaknesses are non-standard parameter naming, an empty JWKS, no scope registry, and\n  the fact that every auth failure arrives as HTTP 200 with a non-zero errorCode.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fxiaoke/refs/heads/main/authentication/fxiaoke-authentication.yml
summary_line: oauth2/custom-token · 4 schemes
tags:
- Company
- Enterprise
- CRM
- Sales
- Marketing
- Customer Service
- SaaS
- China
- PaaS
---
