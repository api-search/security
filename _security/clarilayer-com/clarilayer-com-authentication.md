---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clarilayer-com-openapi-generated.yml
  format: yaml
  label: ClariLayer API
  slug: clarilayer-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/clarilayer-com/openapi/_ae-authored/clarilayer-com-openapi-generated.yml
auth_types: []
description: API v1 Authentication uses API‑key authentication for metric reads. The key is sent in the Authorization header as a Bearer token.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Clarilayer Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClariLayer declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ClariLayer
provider_slug: clarilayer-com
scheme_count: 1
schemes:
- evidence: 'Send the key in the Authorization header: Authorization : Bearer cl_0000000000000000000000000000000000000000'
  header: Authorization
  how_to_obtain: Create an API key via the API‑key management route; the full secret is returned once when the key is created.
  location: header
  name: Authorization
  scopes:
  - canonical-metric-api:read
  - definition:read
  type: apiKey
slug: clarilayer-com-authentication
source_filename: clarilayer-com-authentication.yml
source_heading: Authentication Profile
source_url: https://clarilayer.com/docs/api/v1/authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://clarilayer.com/docs/api/v1/authentication\nsources:\n- https://clarilayer.com/docs/api/v1/authentication\n- https://clarilayer.com/docs/getting-started\n- https://clarilayer.com/docs/quickstart/bootstrap\n- https://clarilayer.com/docs/quickstart/databricks\ndescription: API v1 Authentication uses API‑key authentication for metric reads. The key is sent in the Authorization header as a Bearer token.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'Send the key in the Authorization header: Authorization : Bearer cl_0000000000000000000000000000000000000000'\n  location: header\n  header: Authorization\n  scopes:\n  - canonical-metric-api:read\n  - definition:read\n  how_to_obtain: Create an API key via the API‑key management route; the full secret is returned once when the key is created.\nnote: 'Sandbox keys require an additional header X-ClariLayer-Env: sandbox,\
  \ but the primary authentication scheme is the Bearer API key.'\ndocs: https://clarilayer.com/docs/api/v1/authentication\n"
source_yaml_url: https://artifacts.apis.io/clarilayer-com/authentication/clarilayer-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
