---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Chatmeter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chatmeter declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Chatmeter
provider_slug: chatmeter
scheme_count: 2
schemes:
- description: The value returned by POST /v5/login is placed directly in the Authorization header on subsequent requests. Chatmeter's own product documentation describes this as a JSON Web Token; that claim could not be independently verified from an anonymous probe because issuing a token requires tenant credentials, so the format is recorded as reported, not observed.
  format_reported: JWT
  format_verified: false
  header: Authorization
  id: login-token
  in: header
  scheme: token
  token_endpoint: https://live.chatmeter.com/v5/login
  token_endpoint_content_type: application/json
  token_endpoint_method: POST
  token_request_fields:
  - evidence: POST /v5/login with body {} returns HTTP 400 and {"error":{"code":"INVALID_JSON","message":{"obj.username":[{"msg":["error.path.missing"]}]}}}
    name: username
    required: true
  - evidence: Same 400 response names obj.password with error.path.missing.
    name: password
    required: true
  type: http
- description: GET /v5/singlesignon/generateLoginToken?username=<user> mints a short-lived login token for an existing user, used to hand a browser session to a partner-hosted surface. The route exists and answers 400 (missing parameter) rather than 404 to an anonymous caller, so it is present on the live API, but its token semantics are not publicly documented.
  endpoint: https://live.chatmeter.com/v5/singlesignon/generateLoginToken
  id: sso-login-token
  type: derived-session
slug: chatmeter-authentication
source_filename: chatmeter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: >-\n  Live unauthenticated probes of https://live.chatmeter.com/v5 on 2026-08-13. Chatmeter publishes no\n  OpenAPI, and both of its API documentation hosts are credential-gated (support.chatmeter.com 401 ->\n  Salesforce Community login, apidocs.chatmeter.com 401 with `www-authenticate: Basic`), so the auth\n  profile below is read from what the live API itself returns to an anonymous caller.\nname: Chatmeter API Authentication\napi: Chatmeter API\nbase_url: https://live.chatmeter.com/v5\n\nsummary: >-\n  Username/password token exchange. POST /v5/login with a JSON body of {username, password} returns a\n  token, which is then sent on every subsequent call in the Authorization header. There is no OAuth 2.0,\n  no OIDC discovery document, no self-serve key issuance page, and no public sign-up — credentials are\n  provisioned by Chatmeter for an existing tenant.\n\nschemes:\n  - id: login-token\n    type: http\n    scheme: token\n\
  \    in: header\n    header: Authorization\n    description: >-\n      The value returned by POST /v5/login is placed directly in the Authorization header on subsequent\n      requests. Chatmeter's own product documentation describes this as a JSON Web Token; that claim\n      could not be independently verified from an anonymous probe because issuing a token requires\n      tenant credentials, so the format is recorded as reported, not observed.\n    format_reported: JWT\n    format_verified: false\n    token_endpoint: https://live.chatmeter.com/v5/login\n    token_endpoint_method: POST\n    token_endpoint_content_type: application/json\n    token_request_fields:\n      - name: username\n        required: true\n        evidence: >-\n          POST /v5/login with body {} returns HTTP 400 and\n          {\"error\":{\"code\":\"INVALID_JSON\",\"message\":{\"obj.username\":[{\"msg\":[\"error.path.missing\"]}]}}}\n      - name: password\n        required: true\n        evidence: >-\n      \
  \    Same 400 response names obj.password with error.path.missing.\n\n  - id: sso-login-token\n    type: derived-session\n    description: >-\n      GET /v5/singlesignon/generateLoginToken?username=<user> mints a short-lived login token for an\n      existing user, used to hand a browser session to a partner-hosted surface. The route exists and\n      answers 400 (missing parameter) rather than 404 to an anonymous caller, so it is present on the\n      live API, but its token semantics are not publicly documented.\n    endpoint: https://live.chatmeter.com/v5/singlesignon/generateLoginToken\n\nnot_supported:\n  oauth2: >-\n    No oauth2 flow is offered. /.well-known/oauth-authorization-server and\n    /.well-known/oauth-protected-resource return 302 to the static app bucket on live.chatmeter.com and\n    404 on www.chatmeter.com.\n  openid_connect: >-\n    No /.well-known/openid-configuration on any Chatmeter host.\n  api_keys: >-\n    No self-serve API key page, developer dashboard, or\
  \ key-prefix convention was found on any public\n    Chatmeter surface.\n  mtls: false\n  scopes: >-\n    No scope or permission vocabulary is published. Access is governed by the Chatmeter product's own\n    user/group/location permission model (see /v5/users/{id}/groups and /v5/users/{id}/locations), which\n    is administered in-product rather than declared on the token.\n\nself_serve: false\nself_serve_note: >-\n  There is no public sign-up for API credentials. Chatmeter is sold annually per location through sales;\n  third-party sources place API access in the Premium tier. An integrator cannot obtain a token without\n  an active tenant.\n\nobserved_responses:\n  - request: 'POST https://live.chatmeter.com/v5/login  body {}'\n    status: 400\n    body: '{\"error\":{\"code\":\"INVALID_JSON\",\"message\":{\"obj.password\":[{\"msg\":[\"error.path.missing\"],\"args\":[]}],\"obj.username\":[{\"msg\":[\"error.path.missing\"],\"args\":[]}]}}}'\n  - request: 'GET https://live.chatmeter.com/v5/locations\
  \  (no Authorization header)'\n    status: 401\n    body: '(empty — content-length: 0)'\n    note: >-\n      The 401 carries no body, no WWW-Authenticate header and no error code, so an agent cannot tell a\n      missing token from an expired or insufficiently-privileged one without out-of-band knowledge.\n\ntransport_security:\n  https_only: true\n  hsts: 'max-age=31536000; includeSubDomains'\n  headers_observed:\n    - x-content-type-options: nosniff\n    - referrer-policy: no-referrer\n    - permissions-policy: 'camera=(), microphone=(), geolocation=(), encrypted-media=(), payment=(), speaker=(), usb=()'\n  gateway: istio-envoy\n\ndocs:\n  - url: https://support.chatmeter.com/hc/en-us/categories/4465860037275-Chatmeter-API\n    status: 401\n    note: Redirects to https://support.chatmeter.com/login (Salesforce Experience Cloud community login).\n  - url: https://apidocs.chatmeter.com/\n    status: 401\n    note: 'CloudFront Lambda@Edge HTTP Basic auth (www-authenticate: Basic).'\n\n\
  see_also:\n  - conventions/chatmeter-conventions.yml\n  - errors/chatmeter-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chatmeter/refs/heads/main/authentication/chatmeter-authentication.yml
summary_line: 2 schemes
tags:
- Reputation Management
- Local SEO
- Listings Management
- Review Management
- Social Media
- Multi-Location
- Competitive Intelligence
---
