---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Likeable Local Authentication
name_suffix: Authentication
oauth_flows: []
overview: Likeable Local declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Likeable Local
provider_slug: likeable-local
scheme_count: 2
schemes:
- evidence:
    status: 401
    url: https://api.storytellit.com/users
  id: session-token
  in: unknown
  observed: Anonymous requests to service paths are rejected with HTTP 401 and the body {"name":"NotAuthenticated","message":"You are not authenticated.","code":401, "className":"not-authenticated","errors":{}} — the FeathersJS authentication hook's default rejection. The credential format (JWT bearer, cookie, or Feathers accessToken) is NOT observable without an account, so it is recorded as unknown rather than guessed.
  type: unknown
- evidence:
    status: 200
    url: https://app.storytellit.com/
  id: social-login
  observed: The application bundle references https://api.storytellit.com/social_login/ and the application shell initializes the Facebook JavaScript SDK with a Facebook app id, consistent with the product connecting client Facebook, Instagram and LinkedIn accounts for publishing. This is the company consuming third-party social APIs, not the company issuing credentials to third parties.
  type: oauth2-third-party
slug: likeable-local-authentication
source_filename: likeable-local-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  live unauthenticated HTTP probes of https://api.storytellit.com and https://api.likeablelocal.com,\n  plus the publicly served application bundle\n  https://app.storytellit.com/dist/main-c348e06a35af2239d3e7.js which names the API base\nno_pointer: true\nno_pointer_reason: >-\n  NO `type: Authentication` pointer is wired into apis.yml. The apis.io rating check\n  `authentication_documented` reads `common[].type includes \"Authentication\"` and asserts that the\n  PROVIDER documents authentication as its own topic. Likeable Local / Storytellit publishes no\n  authentication documentation of any kind. This file records what an unauthenticated probe observed\n  about a private backend, which is not the same fact, and wiring the pointer would credit the\n  company with a document it has never published.\nsummary: >-\n  Likeable Local / Storytellit runs a real, live, production API — it is simply not a developer\n  product.\
  \ api.storytellit.com and api.likeablelocal.com resolve to the same AWS application load\n  balancer (prod-api-likeablelocal-1606450325.us-east-2.elb.amazonaws.com) and serve the backend for\n  the login-gated Storytellit / Likeable Local web application. Every service path answers 401 to an\n  anonymous caller. There is no developer portal, no reference, no machine-readable specification,\n  no key issuance flow, and no public sign-up for API access.\napi_surface:\n  discovered: '2026-08-12'\n  base_urls:\n  - https://api.storytellit.com\n  - https://api.likeablelocal.com\n  ownership_evidence: >-\n    The company's own application bundle, served from app.storytellit.com, hard-codes\n    https://api.storytellit.com as its API base and https://api.storytellit.com/social_login/ as its\n    social-login entry point. Both API hostnames CNAME to a single Amazon ELB whose name embeds the\n    company's own product slug (prod-api-likeablelocal). Ownership is not in question.\n  framework_fingerprint:\
  \ >-\n    Express (x-powered-by: Express) fronting FeathersJS — every error body is the FeathersJS envelope\n    {name, message, code, className, errors}, and 404s report className \"not-found\" while 401s report\n    className \"not-authenticated\".\n  public_documentation: none\n  public_specification: none\n  status: private-backend\nschemes:\n- id: session-token\n  type: unknown\n  in: unknown\n  observed: >-\n    Anonymous requests to service paths are rejected with HTTP 401 and the body\n    {\"name\":\"NotAuthenticated\",\"message\":\"You are not authenticated.\",\"code\":401,\n    \"className\":\"not-authenticated\",\"errors\":{}} — the FeathersJS authentication hook's default\n    rejection. The credential format (JWT bearer, cookie, or Feathers accessToken) is NOT observable\n    without an account, so it is recorded as unknown rather than guessed.\n  evidence:\n    url: https://api.storytellit.com/users\n    status: 401\n- id: social-login\n  type: oauth2-third-party\n  observed:\
  \ >-\n    The application bundle references https://api.storytellit.com/social_login/ and the application\n    shell initializes the Facebook JavaScript SDK with a Facebook app id, consistent with the product\n    connecting client Facebook, Instagram and LinkedIn accounts for publishing. This is the company\n    consuming third-party social APIs, not the company issuing credentials to third parties.\n  evidence:\n    url: https://app.storytellit.com/\n    status: 200\ngraphql:\n  endpoint: https://api.storytellit.com/graphql\n  status: gated\n  introspection: refused\n  observed: >-\n    Both GET and a POST introspection query {__schema{queryType{name}}} return HTTP 401 with\n    {\"error\":{\"ok\":false,\"message\":\"Error: User object is required A\",\"data\":{}}} — a distinct\n    envelope from the REST services, so a GraphQL layer is present but the schema cannot be read\n    anonymously. NO SDL has been captured or inferred; nothing about the graph's shape is recorded\n    here because\
  \ nothing about it was observable.\n  evidence:\n    url: https://api.storytellit.com/graphql\n    status: 401\nobserved_error_envelopes:\n- status: 404\n  body: '{\"name\":\"NotFound\",\"message\":\"Page not found\",\"code\":404,\"className\":\"not-found\",\"errors\":{}}'\n- status: 401\n  body: '{\"name\":\"NotAuthenticated\",\"message\":\"You are not authenticated.\",\"code\":401,\"className\":\"not-authenticated\",\"errors\":{}}'\n- status: 401\n  path: /graphql\n  body: '{\"error\":{\"ok\":false,\"message\":\"Error: User object is required A\",\"data\":{}}}'\nnote: >-\n  Recorded so a later round does not repeat the discovery work, and so the profile can state honestly\n  WHY it is thin: this is not a company without an API, it is a company whose API is an internal\n  application backend it has never published, documented, or offered to developers. Nothing in this\n  file was obtained with credentials, and no attempt was made to enumerate the service surface beyond\n  the handful\
  \ of conventional discovery paths every host in this pipeline is probed for.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/likeable-local/refs/heads/main/authentication/likeable-local-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Social-Media
- Marketing
- Social Media Management
- Advertising
- Small Business
- Agencies
- Software-as-a-Service
---
