---
api_key_in:
- config
auth_types:
- apiKey
- http-bearer-jwt
- oauth2
description: 'W4 Cloud authentication model, captured from the W4 Cloud documentation. There is no standalone public REST API with an OpenAPI securitySchemes block — clients authenticate through the w4gd Godot addon. Two layers exist: a project API key that binds the addon to a W4 Cloud workspace, and player authentication handled by a Supabase (GoTrue) identity service issuing JWT bearer tokens used against the database (PostgREST), realtime, and storage services.'
kind: authentication
layout: security
method: searched
name: W4 Games Authentication
name_suffix: Authentication
oauth_flows:
- supabase-social-login
overview: W4 Games secures its APIs with apiKey, http-bearer-jwt, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the supabase-social-login flow(s).
provider_name: W4 Games
provider_slug: w4-games
scheme_count: 3
schemes:
- detail: A per-project/workspace API key issued from the W4 Cloud dashboard (found under DOCS > API). It is set in the w4gd addon configuration to point the Godot client at the correct W4 Cloud workspace/backend.
  in: config
  name: W4 Cloud project API key
  source: https://docs.w4.gd/getting_started/authentication.html
  type: apiKey
- bearerFormat: JWT
  detail: Players authenticate via the Supabase-based identity service (GoTrue), receiving a JWT bearer token. Supported sign-in methods include email/ password, anonymous device login (login_device with a per-user UUID and a key/password), and social OAuth providers configured on the workspace. The JWT authorizes calls to the Supabase-backed database (PostgREST), realtime, and storage layers via the SDK (supabase/auth.gd, supabase/identity.gd, supabase/jwt_utils.gd).
  name: Player authentication (Supabase JWT)
  scheme: bearer
  source: https://docs.w4.gd/getting_started/authentication.html
  type: http
- bearerFormat: JWT
  detail: smauth (addons/w4gd/smauth) provides server-managed authentication so an authoritative dedicated server can synchronize and validate players against W4 Cloud.
  name: Server-managed auth (smauth)
  scheme: bearer
  source: https://docs.w4.gd/api/class_addons_w4gd_smauth_smauth_gd.html
  type: http
slug: w4-games-authentication
source_filename: w4-games-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.w4.gd/getting_started/authentication.html\ndocs: https://docs.w4.gd/getting_started/authentication.html\ndescription: >-\n  W4 Cloud authentication model, captured from the W4 Cloud documentation. There\n  is no standalone public REST API with an OpenAPI securitySchemes block —\n  clients authenticate through the w4gd Godot addon. Two layers exist: a project\n  API key that binds the addon to a W4 Cloud workspace, and player authentication\n  handled by a Supabase (GoTrue) identity service issuing JWT bearer tokens used\n  against the database (PostgREST), realtime, and storage services.\nsummary:\n  types: [apiKey, http-bearer-jwt, oauth2]\n  api_key_in: [config]\n  oauth2_flows: [supabase-social-login]\nschemes:\n- name: W4 Cloud project API key\n  type: apiKey\n  in: config\n  detail: >-\n    A per-project/workspace API key issued from the W4 Cloud dashboard (found\n    under DOCS > API). It is set in the w4gd\
  \ addon configuration to point the\n    Godot client at the correct W4 Cloud workspace/backend.\n  source: https://docs.w4.gd/getting_started/authentication.html\n- name: Player authentication (Supabase JWT)\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  detail: >-\n    Players authenticate via the Supabase-based identity service (GoTrue),\n    receiving a JWT bearer token. Supported sign-in methods include email/\n    password, anonymous device login (login_device with a per-user UUID and a\n    key/password), and social OAuth providers configured on the workspace. The\n    JWT authorizes calls to the Supabase-backed database (PostgREST), realtime,\n    and storage layers via the SDK (supabase/auth.gd, supabase/identity.gd,\n    supabase/jwt_utils.gd).\n  source: https://docs.w4.gd/getting_started/authentication.html\n- name: Server-managed auth (smauth)\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  detail: >-\n    smauth (addons/w4gd/smauth) provides server-managed\
  \ authentication so an\n    authoritative dedicated server can synchronize and validate players against\n    W4 Cloud.\n  source: https://docs.w4.gd/api/class_addons_w4gd_smauth_smauth_gd.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/w4-games/refs/heads/main/authentication/w4-games-authentication.yml
summary_line: apiKey/http-bearer-jwt/oauth2 · 3 schemes
tags:
- Company
- Gaming
- Game Development
- Godot
- Multiplayer
- Backend as a Service
- SDK
- Cloud
- Game Servers
- Realtime
---
