---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usero-io-openapi-generated.yml
  format: yaml
  label: Usero API
  slug: usero-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usero-io/openapi/_ae-authored/usero-io-openapi-generated.yml
auth_types: []
description: Authentication is performed by including a `clientId` (starting with `client_`) in the JSON request body.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Usero Authentication
name_suffix: Authentication
oauth_flows: []
overview: Usero declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Usero
provider_slug: usero-io
scheme_count: 1
schemes:
- evidence: One POST. No SDK, no API key. Works from any language, any platform.
  how_to_obtain: Obtain your clientId from the Usero dashboard or the first screen after signing up; it starts with `client_`.
  location: body
  name: clientId
  type: apiKey
slug: usero-io-authentication
source_filename: usero-io-authentication.yml
source_heading: Authentication Profile
source_url: https://usero.io/docs/index.md
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://usero.io/docs/index.md\nsources:\n- https://usero.io/docs/index.md\n- https://usero.io/docs\ndescription: Authentication is performed by including a `clientId` (starting with `client_`) in the JSON request body.\nschemes:\n- type: apiKey\n  name: clientId\n  evidence: One POST. No SDK, no API key. Works from any language, any platform.\n  location: body\n  how_to_obtain: Obtain your clientId from the Usero dashboard or the first screen after signing up; it starts with `client_`.\ndocs: https://usero.io/docs/index.md\n"
source_yaml_url: https://artifacts.apis.io/usero-io/authentication/usero-io-authentication.yml
summary_line: 1 scheme
tags:
- Feedback
- Session Replay
- B2B SaaS
---
