---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Imvu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Together Labs declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Together Labs
provider_slug: imvu
scheme_count: 0
schemes: []
slug: imvu-authentication
source_filename: imvu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: 'https://api.imvu.com (live probes, 2026-08-23) + https://github.com/imvu/imvu-scripting-docs'\nnote: 'Together Labs publishes NO authentication documentation for any developer surface. No\n  Authentication pointer is emitted in apis.yml, because emitting one would credit the company with an\n  auth reference it does not publish. Everything below was observed, not read.'\ndocumented_by_provider: false\nsecurity_schemes: []\nsurfaces:\n- name: IMVU REST API\n  base_url: https://api.imvu.com\n  model: session-cookie (inferred)\n  evidence:\n  - {observation: 'Vary: Accept, Cookie, Authorization', url: 'https://api.imvu.com/', status: 403}\n  - {observation: 'POST /login with an empty JSON body returns 400 LOGIN-005 \"Invalid login credentials\"', url: 'https://api.imvu.com/login', status: 400}\n  - {observation: 'GET /login returns 405 ROUTER-002 \"Method GET does not exist for login\"', url: 'https://api.imvu.com/login', status:\
  \ 405}\n  - {observation: 'A session resource exists at /login/session (404 \"Session does not exist.\" when absent)', url: 'https://api.imvu.com/login/session', status: 404}\n  - {observation: 'No OAuth surface — GET /oauth/token returns REST_DISCOVER_001 \"Service oauth does not exist\"', url: 'https://api.imvu.com/oauth/token', status: 404}\n  - {observation: 'No OIDC discovery — /.well-known/openid-configuration', url: 'https://api.imvu.com/.well-known/openid-configuration', status: 404}\n  anonymous_read:\n    supported: true\n    note: 'A real slice of the API answers with no credentials at all: /product/product-{id} (200),\n      /user/user-{cid} (200), /user (200 empty collection), /room (200 empty collection),\n      /product/{pid}/uml_products (200). Others gate — /room/room-1 returns 401 AUTHENTICATION-005.'\n  key_issuance:\n    available: false\n    note: 'The public developer program that issued API keys was retired.\n      https://developers.imvu.com/ 302s to https://secure.imvu.com/welcome/login/.'\n\
  \  mtls: false\n  api_key_header: null\n- name: IMVU Room Scripting API\n  model: ambient\n  evidence:\n  - {observation: 'Scripts execute server-side under the room owner''s account; no token, key or\n      credential appears anywhere in the published API.', url: 'https://github.com/imvu/imvu-scripting-docs/blob/main/README.md'}\n  authorization_model: 'Capability is bounded by room membership and ownership rather than by scopes: a\n    script may only target current members of the room it runs in; imvu.place_furniture requires the ROOM\n    OWNER to own the furniture product; imvu.send_room_invite for a foreign room requires a CID-ROOMID\n    form and may still fail. The data module has a three-level sharing scope (script / room / account)\n    plus a per-visitor partition, which is the nearest thing to an authorization scope on this surface.'\n  eligibility: 'VIP membership (a Live Room is required to run a script), alpha-gated.'\noauth_scopes: null\noauth_scopes_note: 'Not applicable\
  \ — no OAuth surface exists, so no scopes/ artifact is written.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/imvu/refs/heads/main/authentication/imvu-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Social Networking
- Virtual Worlds
- Metaverse
- Gaming
- Avatars
- Virtual Goods
- Marketplace
- User Generated Content
- Scripting
- Digital Currency
- Blockchain
---
