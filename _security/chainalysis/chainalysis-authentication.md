---
api_key_in: []
auth_types: []
description: Authentication profile for the Chainalysis API surface, established by probing the live hosts rather than from a specification - Chainalysis publishes no anonymous OpenAPI (developers.chainalysis.com/openapi.json returns HTTP 401). Every Chainalysis API is API-key authenticated via a request header. No OAuth 2.0, OpenID Connect or mutual-TLS surface was found on any host, so no scopes/ artifact is emitted.
kind: authentication
layout: security
method: probed
name: Chainalysis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chainalysis declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Chainalysis
provider_slug: chainalysis
scheme_count: 3
schemes:
- applies_to:
  - api: chainalysis:sanctions-screening
    base: https://public.chainalysis.com/api/v1
  evidence:
  - body: WAF/Cloudflare HTML interstitial
    description: Request with NO credential
    http_status: 403
    url: https://public.chainalysis.com/api/v1/address/{address}
  - body: '{ "message":"Invalid API Key" }'
    description: Request with a well-formed but invalid UUID key in X-API-Key
    http_status: 401
    note: The 401 with a JSON body proves X-API-Key is the credential header the service actually reads - an unauthenticated request never reaches the application.
    url: https://public.chainalysis.com/api/v1/address/{address}
  id: sanctions_api_key
  in: header
  name: X-API-Key
  registration: Free. Requested from the public sanctions screening product page; no commercial contract is required.
  registration_url: https://www.chainalysis.com/product/address-screening/
  type: apiKey
- applies_to:
  - api: chainalysis:kyt-api
    base: https://api.chainalysis.com/api/kyt/v2
  confidence: medium
  evidence:
  - body: '{"timestamp":"...","status":403,"error":"Forbidden","path":"/api/kyt/v2/users"}'
    description: Unauthenticated request to a live KYT operation
    http_status: 403
    url: https://api.chainalysis.com/api/kyt/v2/users
  id: kyt_token
  in: header
  name: Token
  note: 'The header NAME could not be confirmed anonymously - the KYT reference is behind the customer login. The path is confirmed live: it returns a structured application-level 403 rather than the host''s 410 catch-all. Header name recorded at medium confidence and should be upgraded from an authenticated docs read.'
  registration: Enterprise contract; key issued in the KYT console at kyt.chainalysis.com.
  type: apiKey
- applies_to:
  - api: chainalysis:address-screening
    base: https://api.chainalysis.com/api/risk/v2
  confidence: medium
  evidence:
  - body: '{"timestamp":"...","path":"/api/risk/v2/entities","status":403,"error":"Forbidden", "requestId":"497459b3","message":"Invalid token"}'
    description: Unauthenticated request to a live Address Screening operation
    http_status: 403
    note: The application's own message is literally "Invalid token", which is direct evidence that the credential is a bearer-style token supplied per request.
    url: https://api.chainalysis.com/api/risk/v2/entities
  id: risk_token
  in: header
  name: Token
  registration: Enterprise contract.
  type: apiKey
slug: chainalysis-authentication
source_filename: chainalysis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: probed\nsource: >-\n  live unauthenticated + bad-credential probes of public.chainalysis.com and\n  api.chainalysis.com, plus https://www.chainalysis.com/llms.txt\ndescription: >-\n  Authentication profile for the Chainalysis API surface, established by probing the live\n  hosts rather than from a specification - Chainalysis publishes no anonymous OpenAPI\n  (developers.chainalysis.com/openapi.json returns HTTP 401). Every Chainalysis API is\n  API-key authenticated via a request header. No OAuth 2.0, OpenID Connect or mutual-TLS\n  surface was found on any host, so no scopes/ artifact is emitted.\nschemes:\n  - id: sanctions_api_key\n    type: apiKey\n    in: header\n    name: X-API-Key\n    applies_to:\n      - api: chainalysis:sanctions-screening\n        base: https://public.chainalysis.com/api/v1\n    registration: >-\n      Free. Requested from the public sanctions screening product page; no commercial\n      contract is required.\n  \
  \  registration_url: https://www.chainalysis.com/product/address-screening/\n    evidence:\n      - description: Request with NO credential\n        url: https://public.chainalysis.com/api/v1/address/{address}\n        http_status: 403\n        body: WAF/Cloudflare HTML interstitial\n      - description: Request with a well-formed but invalid UUID key in X-API-Key\n        url: https://public.chainalysis.com/api/v1/address/{address}\n        http_status: 401\n        body: '{ \"message\":\"Invalid API Key\" }'\n        note: >-\n          The 401 with a JSON body proves X-API-Key is the credential header the service\n          actually reads - an unauthenticated request never reaches the application.\n  - id: kyt_token\n    type: apiKey\n    in: header\n    name: Token\n    applies_to:\n      - api: chainalysis:kyt-api\n        base: https://api.chainalysis.com/api/kyt/v2\n    registration: Enterprise contract; key issued in the KYT console at kyt.chainalysis.com.\n    confidence: medium\n\
  \    evidence:\n      - description: Unauthenticated request to a live KYT operation\n        url: https://api.chainalysis.com/api/kyt/v2/users\n        http_status: 403\n        body: >-\n          {\"timestamp\":\"...\",\"status\":403,\"error\":\"Forbidden\",\"path\":\"/api/kyt/v2/users\"}\n    note: >-\n      The header NAME could not be confirmed anonymously - the KYT reference is behind the\n      customer login. The path is confirmed live: it returns a structured application-level\n      403 rather than the host's 410 catch-all. Header name recorded at medium confidence\n      and should be upgraded from an authenticated docs read.\n  - id: risk_token\n    type: apiKey\n    in: header\n    name: Token\n    applies_to:\n      - api: chainalysis:address-screening\n        base: https://api.chainalysis.com/api/risk/v2\n    registration: Enterprise contract.\n    confidence: medium\n    evidence:\n      - description: Unauthenticated request to a live Address Screening operation\n  \
  \      url: https://api.chainalysis.com/api/risk/v2/entities\n        http_status: 403\n        body: >-\n          {\"timestamp\":\"...\",\"path\":\"/api/risk/v2/entities\",\"status\":403,\"error\":\"Forbidden\",\n          \"requestId\":\"497459b3\",\"message\":\"Invalid token\"}\n        note: >-\n          The application's own message is literally \"Invalid token\", which is direct\n          evidence that the credential is a bearer-style token supplied per request.\nnot_found:\n  oauth2: >-\n    No oauth2 securityScheme, no /.well-known/oauth-authorization-server (404 on\n    www.chainalysis.com; SPA shell on reactor.chainalysis.com), no documented authorization\n    or token endpoint. scopes/ is deliberately NOT emitted.\n  openid_connect: >-\n    No /.well-known/openid-configuration served on any host (404 / SPA shell).\n  mutual_tls: Not documented and not offered on any probed host.\ndocs: https://developers.chainalysis.com/\ndocs_status: 401\ndocs_note: >-\n  The Chainalysis\
  \ developer portal is entirely behind a customer login. Every content path\n  returns the literal body \"User is not logged in\" and /openapi.json returns\n  {\"error\":\"Unauthorized\"}. The auth model above is therefore probed, not read.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chainalysis/refs/heads/main/authentication/chainalysis-authentication.yml
summary_line: 3 schemes
tags:
- Compliance
- AML
- KYT
- Sanctions
- Investigations
- Blockchain Analytics
- Risk
- Crypto
---
