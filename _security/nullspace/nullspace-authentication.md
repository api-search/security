---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nullspace-openapi-generated.yml
  format: yaml
  label: Nullspace API
  slug: nullspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nullspace/openapi/_ae-authored/nullspace-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nullspace Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nullspace declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nullspace
provider_slug: nullspace
scheme_count: 1
schemes:
- evidence: Authorization string header required Supabase Auth access token passed as Bearer token
  header: Authorization
  how_to_obtain: Supabase Auth access token
  location: header
  name: Authorization
  type: http-bearer
slug: nullspace-authentication
source_filename: nullspace-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.ns.rocks/api-reference/api-keys/create-an-api-key-for-the-authenticated-user
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.ns.rocks/api-reference/api-keys/create-an-api-key-for-the-authenticated-user\nsources:\n- https://docs.ns.rocks/api-reference/api-keys/create-an-api-key-for-the-authenticated-user\n- https://docs.ns.rocks/api-reference/api-keys/idempotently-create-the-first-runtime-api-key\n- https://docs.ns.rocks/api-reference/api-keys/list-api-keys-for-the-authenticated-user\n- https://docs.ns.rocks/api-reference/api-keys/revoke-an-api-key\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: Authorization string header required Supabase Auth access token passed as Bearer token\n  location: header\n  header: Authorization\n  how_to_obtain: Supabase Auth access token\ndocs: https://docs.ns.rocks/api-reference/api-keys/create-an-api-key-for-the-authenticated-user\n"
source_yaml_url: https://artifacts.apis.io/nullspace/authentication/nullspace-authentication.yml
summary_line: 1 scheme
tags:
- Cloud Infrastructure
- AI Agents
---
