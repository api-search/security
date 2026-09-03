---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Turion Space Authentication
name_suffix: Authentication
oauth_flows: []
overview: Turion Space declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Turion Space
provider_slug: turion-space
scheme_count: 2
schemes:
- confidence: medium
  discovery_document: null
  evidence: 'app.turionspace.com is titled "Turion Space: Authentication" and its bundle carries Ory (OAuth2/OIDC) client code; the STARFIRE dashboard bundle calls https://api.app.turionspace.com/api/v1/auth. The grant types, authorization/token endpoints, issuer and scopes are NOT discoverable anonymously — no OIDC discovery document is served on any Turion host (see well-known/turion-space-well-known.yml).'
  id: starfire-session
  type: oauth2
- confidence: medium
  evidence: The STARFIRE dashboard bundle contains the route "/api/v1/users/api-key", indicating the product issues per-user API keys from within the authenticated dashboard. The header or query parameter the key is presented in, its prefix, its lifetime and its revocation semantics are all undocumented and were NOT observed.
  header: unknown
  id: starfire-api-key
  prefix: unknown
  type: apiKey
slug: turion-space-authentication
source_filename: turion-space-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  https://app.turionspace.com/config.js (the provider's own runtime configuration, served\n  unauthenticated) and the provider's own published dashboard bundles\n  https://starfire.turionspace.com/assets/index-Bvr-pAIX.js and\n  https://app.turionspace.com/assets/index-CV8WCmB3.js\nnote: >-\n  Turion Space publishes NO authentication documentation of any kind. Everything below is observed\n  from first-party assets the provider serves anonymously, not from a documented auth reference. It\n  is recorded so the gap is legible; it is NOT a substitute for the provider publishing an auth page,\n  and no `Authentication` pointer is emitted in apis.yml because the check it feeds asks whether the\n  PROVIDER documents authentication, and they do not.\ndocumented_publicly: false\napi: Turion Space STARFIRE API\nbase_url: https://api.app.turionspace.com\nschemes:\n- id: starfire-session\n  type: oauth2\n  confidence: medium\n  evidence:\
  \ >-\n    app.turionspace.com is titled \"Turion Space: Authentication\" and its bundle carries Ory\n    (OAuth2/OIDC) client code; the STARFIRE dashboard bundle calls\n    https://api.app.turionspace.com/api/v1/auth. The grant types, authorization/token endpoints,\n    issuer and scopes are NOT discoverable anonymously — no OIDC discovery document is served on any\n    Turion host (see well-known/turion-space-well-known.yml).\n  discovery_document: null\n- id: starfire-api-key\n  type: apiKey\n  confidence: medium\n  evidence: >-\n    The STARFIRE dashboard bundle contains the route \"/api/v1/users/api-key\", indicating the product\n    issues per-user API keys from within the authenticated dashboard. The header or query parameter\n    the key is presented in, its prefix, its lifetime and its revocation semantics are all\n    undocumented and were NOT observed.\n  header: unknown\n  prefix: unknown\nanonymous_behaviour:\n  probe: GET https://api.app.turionspace.com/api/v1/tasking-orders\n\
  \  status: 404\n  body: '{\"error_msg\":\"404 Route Not Found\"}'\n  interpretation: >-\n    The gateway does not distinguish an unauthenticated caller from an unknown route; it returns a\n    generic Go/Echo 404 envelope rather than a 401 with a WWW-Authenticate challenge. An agent cannot\n    tell from the wire whether it lacks credentials or asked for a path that does not exist.\ngaps:\n- No public authentication reference page.\n- No OIDC/OAuth discovery document on any host.\n- No documented scopes; scopes/ is intentionally not written.\n- No 401 challenge or WWW-Authenticate header on the public gateway.\n- No documented API key header, prefix, rotation or revocation policy.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turion-space/refs/heads/main/authentication/turion-space-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Space
- Satellites
- Space Domain Awareness
- Non-Earth Imaging
- Earth Observation
- Aerospace
- Defense
- Geospatial
- Imagery
---
