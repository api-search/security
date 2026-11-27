---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nifra-dev-openapi-generated.yml
  format: yaml
  label: Nifra API
  slug: nifra-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nifra-dev/openapi/_ae-authored/nifra-dev-openapi-generated.yml
auth_types: []
description: Authentication mechanisms described in Nifra documentation
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Nifra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nifra declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Nifra
provider_slug: nifra-dev
scheme_count: 2
schemes:
- evidence: betterAuth(auth) mounts its handler at /api/auth/* (GET + POST), so every endpoint - sign-in/up/out, OAuth callbacks, session, 2FA, magic links - is served by your Nifra server.
  name: Better Auth
  type: oauth2
- evidence: authjs(config) serves /api/auth/* (sign-in, OAuth callbacks, session, sign-out, CSRF) through @auth/core itself.
  name: Auth.js
  type: oauth2
slug: nifra-dev-authentication
source_filename: nifra-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://nifra.dev/docs/auth
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nifra.dev/docs/auth\nsources:\n- https://nifra.dev/docs/auth\n- https://nifra.dev/docs\ndescription: Authentication mechanisms described in Nifra documentation\nschemes:\n- type: oauth2\n  name: Better Auth\n  evidence: betterAuth(auth) mounts its handler at /api/auth/* (GET + POST), so every endpoint - sign-in/up/out, OAuth callbacks, session, 2FA,\n    magic links - is served by your Nifra server.\n- type: oauth2\n  name: Auth.js\n  evidence: authjs(config) serves /api/auth/* (sign-in, OAuth callbacks, session, sign-out, CSRF) through @auth/core itself.\ndocs: https://nifra.dev/docs/auth\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/nifra-dev/authentication/nifra-dev-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- TypeScript
- Framework
- Full-Stack
- Open Source
---
