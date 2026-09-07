---
anonymous_access: false
api_key_in: []
api_specs:
- filename: anew-openapi.json
  format: json
  label: anew Write/Read API
  slug: anew-writeread-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anew/refs/heads/main/openapi/anew-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Anew Authentication
name_suffix: Authentication
oauth_flows: []
overview: anew declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: anew
provider_slug: anew
scheme_count: 0
schemes: []
slug: anew-authentication
source_filename: anew-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: 'https://anew.page/llms.txt (the Authentication-none statement) + openapi/anew-openapi.json (security: [{}])'\ndocs: https://anew.page/llms.txt\nsummary: >-\n  anew publishes no authentication of any kind. Every endpoint is public and unauthenticated — no API\n  key, no OAuth, no bearer token, no signup, no account. The OpenAPI states this positively rather than\n  by omission: a top-level `security: [{}]` and an empty `components.securitySchemes`. The docs restate\n  it as an instruction to callers: \"Do not send credentials; nothing reads them.\"\nauth_required: false\nsecurity_schemes: []\nschemes_declared_in_spec: 0\nspec_security: '[{}]'\nnotes:\n  - >-\n    `security: [{}]` is the explicit OpenAPI 3.1 idiom for \"this operation may be called with no\n    security\". It is materially different from a spec that simply omits `security`, which is ambiguous.\n    anew declares the absence deliberately.\n  - >-\n    There is\
  \ no account system, so there is no signup, login, key rotation, key prefix, or scope surface.\n    scopes/ is therefore not applicable and is deliberately absent from this repo.\n  - >-\n    The only request-shaping controls are transport-level, not identity-level: /mcp validates the browser\n    `Origin` header per the MCP specification and answers 403 `origin_forbidden` for an opaque, insecure\n    or non-canonical Origin. /write and /a2a/v1 are not Origin-gated and answer CORS `*`.\n  - >-\n    anew serves an RFC 9421 HTTP Message Signatures directory at\n    /.well-known/http-message-signatures-directory carrying one Ed25519 signing key. This is a key for\n    verifying signatures anew produces, not a caller authentication requirement.\naccess_control:\n  cors:\n    allow_origin: '*'\n    allow_methods: [POST, OPTIONS]\n    expose_headers: [Anew-URL-Bytes, Anew-URL-Limit, Anew-Decoded-Bytes, Anew-Decoded-Limit, Anew-Share-Warning, RateLimit-Policy]\n    max_age: 86400\n    observed:\
  \ '2026-09-04 on POST https://anew.page/write (HTTP 200)'\n  origin_gated_endpoints:\n    - endpoint: https://anew.page/mcp\n      behavior: 403 origin_forbidden for opaque/insecure/non-canonical browser Origin\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anew/refs/heads/main/authentication/anew-authentication.yml
summary_line: 0 schemes
tags:
- html
- webpage
- website
- url
- encode
- share
- web-publishing
- developer-tools
- mcp
- a2a
- ai-agent-tooling
- llms-txt
- agents-txt
- agent-skills
- webmcp
- openapi
- stateless
- immutable
- no-auth
- static-site
- url-encoding
---
