---
anonymous_access: false
api_key_in: []
api_specs:
- filename: instavision-co-openapi-generated.yml
  format: yaml
  label: InstaVision API
  slug: instavision-co-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/instavision-co/openapi/_ae-authored/instavision-co-openapi-generated.yml
auth_types: []
description: Authentication methods for InstaVision as described in the documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: InstaVision Authentication
name_suffix: Authentication
oauth_flows: []
overview: InstaVision declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: InstaVision
provider_slug: instavision-co
scheme_count: 1
schemes:
- evidence: 'An API key (from a registration, or from the person): `Authorization: Bearer <key>` (or `X-API-Key: <key>`) on `https://instavision.co/api/mcp/mcp`.'
  header: Authorization
  how_to_obtain: Create an API key in the InstaVision UI at https://instavision.co/settings/api-keys or obtain it via the service_auth or anonymous registration flows.
  name: API key / OAuth access token
  type: http-bearer
slug: instavision-co-authentication
source_filename: instavision-co-authentication.yml
source_heading: Authentication Profile
source_url: https://instavision.co/login?next=%2Fsettings%2Fapi-keys
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://instavision.co/login?next=%2Fsettings%2Fapi-keys\nsources:\n- https://instavision.co/login?next=%2Fsettings%2Fapi-keys\n- https://instavision.co/auth.md\n- https://instavision.co/agents.md\n- https://instavision.co/mcp\ndescription: Authentication methods for InstaVision as described in the documentation.\nschemes:\n- type: http-bearer\n  name: API key / OAuth access token\n  evidence: 'An API key (from a registration, or from the person): `Authorization: Bearer <key>` (or `X-API-Key: <key>`) on `https://instavision.co/api/mcp/mcp`.'\n  header: Authorization\n  how_to_obtain: Create an API key in the InstaVision UI at https://instavision.co/settings/api-keys or obtain it via the service_auth or anonymous\n    registration flows.\ndocs: https://instavision.co/login?next=%2Fsettings%2Fapi-keys\nnote: 3 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/instavision-co/authentication/instavision-co-authentication.yml
summary_line: 1 scheme
tags:
- B2B
- Instagram
- Artificial Intelligence
- Discovery
- Marketing
---
