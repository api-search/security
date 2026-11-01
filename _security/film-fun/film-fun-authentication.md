---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Splice accepts two credentials: an OAuth 2.1 access token (authorization code + PKCE) and an agent key (sk_…) used as a bearer token.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Film Fun Authentication
name_suffix: Authentication
oauth_flows: []
overview: film-fun declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: film-fun
provider_slug: film-fun
scheme_count: 2
schemes:
- authorize_url: https://splice.film.fun/oauth/authorize
  evidence: 'Splice (https://splice.film.fun) accepts two credentials, both acting as one Splice user and spending that user''s credits: - an **OAuth 2.1 access token** (authorization code + PKCE, with dynamic client registration), for clients that can send the user to a browser once;'
  flows:
  - authorization_code
  how_to_obtain: Register a public client via dynamic registration (POST /oauth/register) to get a client_id, then send the user to the authorize URL with PKCE and the desired scopes, receive an authorization code, and exchange it at the token endpoint (POST /oauth/token) for an access token.
  name: OAuth 2.1 access token
  scopes:
  - splice:read
  - splice:generate
  - splice:compose
  - splice:produce
  type: http-bearer
- evidence: The user gave you an agent key (`sk_…`) → skip to [Step 6](#step-6--use-the-credential).
  how_to_obtain: Create an API key in the user dashboard at https://splice.film.fun/dashboard/api-keys and use the returned `sk_…` value as a Bearer token.
  name: Agent key
  type: http-bearer
slug: film-fun-authentication
source_filename: film-fun-authentication.yml
source_heading: Authentication Profile
source_url: https://splice.film.fun/auth.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://splice.film.fun/auth.md\nsources:\n- https://splice.film.fun/auth.md\ndescription: 'Splice accepts two credentials: an OAuth 2.1 access token (authorization code + PKCE) and an agent key (sk_…) used as a bearer token.'\nschemes:\n- type: http-bearer\n  name: OAuth 2.1 access token\n  evidence: 'Splice (https://splice.film.fun) accepts two credentials, both acting as one Splice user and spending that user''s credits: - an\n    **OAuth 2.1 access token** (authorization code + PKCE, with dynamic client registration), for clients that can send the user to a browser\n    once;'\n  flows:\n  - authorization_code\n  authorize_url: https://splice.film.fun/oauth/authorize\n  scopes:\n  - splice:read\n  - splice:generate\n  - splice:compose\n  - splice:produce\n  how_to_obtain: Register a public client via dynamic registration (POST /oauth/register) to get a client_id, then send the\
  \ user to the authorize\n    URL with PKCE and the desired scopes, receive an authorization code, and exchange it at the token endpoint (POST /oauth/token) for an access\n    token.\n- type: http-bearer\n  name: Agent key\n  evidence: The user gave you an agent key (`sk_…`) → skip to [Step 6](#step-6--use-the-credential).\n  how_to_obtain: Create an API key in the user dashboard at https://splice.film.fun/dashboard/api-keys and use the returned `sk_…` value as a\n    Bearer token.\ndocs: https://splice.film.fun/auth.md\n"
source_yaml_url: https://artifacts.apis.io/film-fun/authentication/film-fun-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- VideoEditing
- Filmmaking
- Platform
---
