---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Rosettaai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rosetta.ai declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Rosetta.ai
provider_slug: rosettaai
scheme_count: 0
schemes: []
slug: rosettaai-authentication
source_filename: rosettaai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: derived\nsource: https://cdn.rosetta.ai/rosetta.min.js\ndocs: null\nprovenance_note: >-\n  DERIVED FROM FIRST-PARTY SHIPPED CODE, NOT FROM DOCUMENTATION. Rosetta.ai\n  publishes no authentication page, no API reference and no OpenAPI. Everything\n  below was read directly out of Rosetta.ai's own production on-site tag,\n  https://cdn.rosetta.ai/rosetta.min.js (HTTP 200, 47,751 bytes, VERSION=\"2.0.0\"),\n  which is served from a hostname Rosetta.ai controls and is the exact file its\n  merchants load. It is recorded as an observation of a real, live auth scheme —\n  it is NOT a claim that Rosetta.ai documents any of this, and no spec has been\n  synthesised from it.\napi_host: https://api.rosetta.ai\napi_host_status: >-\n  Live. Resolves to 146.190.4.25 (DigitalOcean), Laravel application, HTTP/2,\n  HSTS max-age=15724800; includeSubDomains. Returns a genuine Laravel 404 for\n  unknown paths and 204 for /sanctum/csrf-cookie, which is what identifies\
  \ the\n  stack.\npublic_developer_program: false\nsecurity_schemes:\n- id: bearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer <token>'\n  evidence: >-\n    axios instance constructed in rosetta.min.js with\n    headers:{Authorization:`Bearer ${e}`} against baseURL \"https://api.rosetta.ai/\".\n  token_issuance: >-\n    Not observable anonymously. The v2 tag receives its token from the surrounding\n    page configuration. A newer (and currently DEAD — see packages/) bundle,\n    rosetta-web.js, calls POST /api/user/issue-token to mint one, which indicates a\n    token-issuance endpoint exists on the API, but that bundle points at\n    v4-api.rosetta.ai, which does not resolve.\n  scopes: none-observed\n  rotation_policy: not-published\n  expiry: not-published\n- id: sessionCookie\n  type: cookie\n  scheme: laravel-sanctum\n  evidence: >-\n    https://api.rosetta.ai/sanctum/csrf-cookie returns HTTP 204, and\n    https://api.rosetta.ai/login\
  \ returns HTTP 200. This is Laravel Sanctum's\n    SPA/cookie session flow, used by the dashboard.rosetta.ai front end rather\n    than by any third-party integrator.\n  public: false\noauth2: false\nopenid_connect: false\nmutual_tls: false\napi_keys_self_service: false\ncontent_negotiation:\n  accept: application/vnd.rosetta-ai.v2+json\n  note: >-\n    The tag pins the API version through a vendor media type in the Accept header\n    rather than through a URL path segment. See conventions/.\nobserved_operations:\n- method: POST\n  path: /entity\n  body_fields: [name, id, fingerprint, type]\n  purpose: identify or create an actor (visitor/user), keyed by browser fingerprint\n- method: POST\n  path: /entity/local_retrieval\n  body_fields: [local_id]\n  purpose: resolve a locally stored identifier back to an entity\n- method: GET\n  path: /entity/{item}\n  purpose: retrieve a single entity\n- method: POST\n  path: /event\n  body_fields: [actor, action, target]\n  purpose: behavioural event\
  \ ingest (actor/action/target triple)\n- method: POST\n  path: /engine/{engineID}/query\n  body_fields: [user, item]\n  purpose: request recommendations from a named recommendation engine\nobserved_operations_note: >-\n  These are the request paths the production tag actually issues. They are recorded\n  as evidence of the shape of the auth surface. NO OpenAPI has been written from\n  them and none should be: an operation list reverse-read from a minified bundle is\n  an observation, not a contract the provider published, and turning it into a spec\n  would manufacture a developer surface Rosetta.ai does not offer.\npointer_decision:\n  emit_authentication_pointer: false\n  reason: >-\n    Deliberately NOT wired as `type: Authentication` in apis.yml. That pointer feeds\n    the `authentication_documented` check, and Rosetta.ai documents nothing — this\n    file exists only because the scheme could be read out of shipped code. Emitting\n    the pointer would convert our reverse-reading\
  \ into the provider's documentation\n    and award points for a page that does not exist. The artifact stays in the repo\n    as evidence; the pointer is withheld until Rosetta.ai publishes an auth page.\ngaps:\n- No published authentication documentation of any kind.\n- No self-service API credential issuance; no API keys page in the dashboard docs.\n- No token lifetime, refresh or revocation policy published.\n- No OAuth 2.0, OIDC or scope model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rosettaai/refs/heads/main/authentication/rosettaai-authentication.yml
summary_line: 0 schemes
tags:
- Company
- E-commerce
- Personalization
- Recommendations
- Marketing Automation
- Artificial Intelligence
- Retail
- Shopify
- Machine Learning
- Conversion Optimization
---
