---
anonymous_access: false
api_key_in: []
api_specs:
- filename: shipyard-openapi-generated.yml
  format: yaml
  label: Shipyard API
  slug: shipyard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/shipyard/openapi/_ae-authored/shipyard-openapi-generated.yml
auth_types: []
description: Authentication for Shipyard environments
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Shipyard Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shipyard declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Shipyard
provider_slug: shipyard
scheme_count: 1
schemes:
- evidence: 'Make a request to your environment url with a `shipyard_token` query arg and your `bypass_token` as the value:'
  how_to_obtain: Copy the `bypass_token` from the Visitors page for the specific environment (via the three‑dot menu on the developer dashboard).
  location: query
  name: bypass_token
  type: apiKey
slug: shipyard-authentication
source_filename: shipyard-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.stackgen.com/shipyard/environments/configuration/authentication.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.stackgen.com/shipyard/environments/configuration/authentication.md\nsources:\n- https://docs.stackgen.com/shipyard/environments/configuration/authentication.md\n- https://docs.stackgen.com/docs/release-notes/stackgen-platform/2026/august/v2026-8-3.md\n- https://docs.stackgen.com/docs/release-notes/stackgen-platform/2026/july/v2026-7-7.md\n- https://docs.stackgen.com/docs/release-notes/stackgen-platform/2026/september/v2026-9-7.md\ndescription: Authentication for Shipyard environments\nschemes:\n- type: apiKey\n  name: bypass_token\n  evidence: 'Make a request to your environment url with a `shipyard_token` query arg and your `bypass_token` as the value:'\n  location: query\n  how_to_obtain: Copy the `bypass_token` from the Visitors page for the specific environment (via the three‑dot menu on the developer dashboard).\nnote: The documentation does not describe any OAuth\
  \ flows, HTTP bearer, basic, JWT, HMAC, mTLS, or other schemes.\ndocs: https://docs.stackgen.com/shipyard/environments/configuration/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/shipyard/authentication/shipyard-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Ephemeral Environments
- CI/CD
- DevOps
- AI Agents
---
