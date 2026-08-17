---
api_key_in: []
auth_types:
- http
description: Authentication profile for the ReviewTrackers REST API, established by probing the live production host rather than from an OpenAPI document — ReviewTrackers publishes no machine-readable specification and its developer portal is credential-gated. Every protected resource answers an anonymous request with HTTP 401 and an HTTP Basic challenge; there is a dedicated /auth token-exchange endpoint that accepts a set of vendored JSON media types.
kind: authentication
layout: security
method: probed
name: Reviewtrackers Authentication
name_suffix: Authentication
oauth_flows: []
overview: ReviewTrackers secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ReviewTrackers
provider_slug: reviewtrackers
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Every protected collection returns WWW-Authenticate Basic realm="rtx:production" to an anonymous caller.
  evidence:
  - body: '{"error":"Must Be Authenticated.","status":401}'
    request: GET https://api.reviewtrackers.com/accounts
    status: 401
    www_authenticate: Basic realm="rtx:production"
  - request: GET https://api.reviewtrackers.com/locations
    status: 401
    www_authenticate: Basic realm="rtx:production"
  - request: GET https://api.reviewtrackers.com/users
    status: 401
    www_authenticate: Basic realm="rtx:production"
  in: header
  name: basic
  parameter: Authorization
  realm: rtx:production
  scheme: basic
  type: http
slug: reviewtrackers-authentication
source_filename: reviewtrackers-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  Live unauthenticated requests to https://api.reviewtrackers.com/ (root, /auth,\n  /accounts, /reviews, /locations, /users) on 2026-08-13\ndocs: https://developer.reviewtrackers.com/\nname: ReviewTrackers API Authentication\ndescription: >-\n  Authentication profile for the ReviewTrackers REST API, established by probing\n  the live production host rather than from an OpenAPI document — ReviewTrackers\n  publishes no machine-readable specification and its developer portal is\n  credential-gated. Every protected resource answers an anonymous request with\n  HTTP 401 and an HTTP Basic challenge; there is a dedicated /auth token-exchange\n  endpoint that accepts a set of vendored JSON media types.\nsummary:\n  types:\n    - http\n  http_schemes:\n    - basic\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n  - name: basic\n    type: http\n    scheme: basic\n   \
  \ realm: rtx:production\n    in: header\n    parameter: Authorization\n    description: >-\n      HTTP Basic authentication. Every protected collection returns\n      WWW-Authenticate Basic realm=\"rtx:production\" to an anonymous caller.\n    evidence:\n      - request: GET https://api.reviewtrackers.com/accounts\n        status: 401\n        www_authenticate: Basic realm=\"rtx:production\"\n        body: '{\"error\":\"Must Be Authenticated.\",\"status\":401}'\n      - request: GET https://api.reviewtrackers.com/locations\n        status: 401\n        www_authenticate: Basic realm=\"rtx:production\"\n      - request: GET https://api.reviewtrackers.com/users\n        status: 401\n        www_authenticate: Basic realm=\"rtx:production\"\ntoken_exchange:\n  endpoint: https://api.reviewtrackers.com/auth\n  method: POST\n  description: >-\n    Credential exchange endpoint. Rejects a request with no Content-Type with HTTP\n    415, enumerating the exact media types it accepts; rejects a request\
  \ with no\n    credentials with HTTP 401 and the Basic challenge. The token format returned\n    on success is documented only inside the gated developer portal and was not\n    observed in this pass.\n  accepted_content_types:\n    - application/json\n    - application/json;charset=utf-8\n    - application/hal+json\n    - application/hal+json;charset=utf-8\n    - application/vnd.rtx.hal+json\n    - application/vnd.rtx.hal+json;charset=utf-8\n    - application/vnd.rtx.auth.hal+json\n    - application/vnd.rtx.auth.hal+json;charset=utf-8\n    - application/vnd.rtx.v2.hal+json\n    - application/vnd.rtx.v2.hal+json;charset=utf-8\n    - application/vnd.rtx.auth.v2.hal+json\n    - application/vnd.rtx.auth.v2.hal+json;charset=utf-8\n  evidence:\n    - request: POST https://api.reviewtrackers.com/auth (no Content-Type)\n      status: 415\n      body_excerpt: 'Unsupported content type \"\"; expected one of [...]'\n    - request: POST https://api.reviewtrackers.com/auth (Content-Type application/json,\
  \ empty body)\n      status: 401\n      content_type: application/vnd.rtx.auth.v2.hal+json;charset=utf-8\n      www_authenticate: Basic realm=\"rtx:production\"\nkey_management:\n  self_service: false\n  note: >-\n    API credentials are not self-service. The API root itself responds\n    {\"message\":\"Contact your CS representative or reference\n    https://developer.reviewtrackers.com/\"} — credentials are issued by a customer\n    success representative, and API access is a plan entitlement (see\n    plans/reviewtrackers-plans-pricing.yml).\nnotes:\n  - No OAuth 2.0, OpenID Connect, or API-key scheme was observed; there is therefore\n    no scopes/ artifact for this provider.\n  - >-\n    No /.well-known/oauth-authorization-server or /.well-known/openid-configuration\n    is served on any host (see well-known/reviewtrackers-well-known.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reviewtrackers/refs/heads/main/authentication/reviewtrackers-authentication.yml
summary_line: http · 1 scheme
tags:
- Reputation Management
- Review Monitoring
- Customer Feedback
- Sentiment Analytics
- Local SEO
- Online Reviews
- Multi-Location
- Customer Experience
- Review Response
- Local Listings
---
