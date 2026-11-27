---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nanotoll-dev-account-api-openapi.yml
  format: yaml
  label: Nanotoll Account API
  slug: nanotoll-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanotoll-dev/openapi/nanotoll-dev-account-api-openapi.yml
- filename: nanotoll-dev-operational-api-openapi.yml
  format: yaml
  label: Nanotoll Operational API
  slug: nanotoll-dev-operational-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanotoll-dev/openapi/nanotoll-dev-operational-api-openapi.yml
auth_types: []
description: Nanotoll authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nanotoll Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nanotoll declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nanotoll
provider_slug: nanotoll-dev
scheme_count: 1
schemes:
- evidence: 'All billing endpoints require a Bearer token: Authorization: Bearer macs_a1b2...c5d6'
  header: Authorization
  how_to_obtain: Register via POST /api/v1/register (no auth, no body) – the response contains your API key which is used as the Bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: nanotoll-dev-authentication
source_filename: nanotoll-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://nanotoll.dev/docs/getting-started/authentication/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nanotoll.dev/docs/getting-started/authentication/\nsources:\n- https://nanotoll.dev/docs/getting-started/authentication/\n- https://nanotoll.dev/docs/getting-started/\n- https://nanotoll.dev/docs/getting-started/billing/\ndescription: Nanotoll authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'All billing endpoints require a Bearer token: Authorization: Bearer macs_a1b2...c5d6'\n  location: header\n  header: Authorization\n  how_to_obtain: Register via POST /api/v1/register (no auth, no body) – the response contains your API key which is used as the Bearer token.\ndocs: https://nanotoll.dev/docs/getting-started/authentication/\n"
source_yaml_url: https://artifacts.apis.io/nanotoll-dev/authentication/nanotoll-dev-authentication.yml
summary_line: 1 scheme
tags:
- LLM
- Compression
- USDC
- Base
---
