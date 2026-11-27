---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gemot-dev-a2a-api-openapi.yml
  format: yaml
  label: Gemot A2a API
  slug: gemot-dev-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-a2a-api-openapi.yml
- filename: gemot-dev-balance-api-openapi.yml
  format: yaml
  label: Gemot Balance API
  slug: gemot-dev-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-balance-api-openapi.yml
- filename: gemot-dev-checkout-api-openapi.yml
  format: yaml
  label: Gemot Checkout API
  slug: gemot-dev-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-checkout-api-openapi.yml
- filename: gemot-dev-events-api-openapi.yml
  format: yaml
  label: Gemot Events API
  slug: gemot-dev-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-events-api-openapi.yml
- filename: gemot-dev-export-api-openapi.yml
  format: yaml
  label: Gemot Export API
  slug: gemot-dev-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-export-api-openapi.yml
- filename: gemot-dev-health-api-openapi.yml
  format: yaml
  label: Gemot Health API
  slug: gemot-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-health-api-openapi.yml
- filename: gemot-dev-join-api-openapi.yml
  format: yaml
  label: Gemot Join API
  slug: gemot-dev-join-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-join-api-openapi.yml
- filename: gemot-dev-oauth-api-openapi.yml
  format: yaml
  label: Gemot OAuth API
  slug: gemot-dev-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-oauth-api-openapi.yml
- filename: gemot-dev-try-api-openapi.yml
  format: yaml
  label: Gemot Try API
  slug: gemot-dev-try-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-try-api-openapi.yml
- filename: gemot-dev-well-known-api-openapi.yml
  format: yaml
  label: Gemot .well Known API
  slug: gemot-dev-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gemot-dev/openapi/gemot-dev-well-known-api-openapi.yml
auth_types: []
description: Authentication methods as published on Gemot pages
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Gemot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gemot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Gemot
provider_slug: gemot-dev
scheme_count: 1
schemes:
- evidence: The join_code authenticates sandbox access.
  location: body
  name: join_code
  type: apiKey
slug: gemot-dev-authentication
source_filename: gemot-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://gemot.dev/.well-known/oauth-authorization-server
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gemot.dev/.well-known/oauth-authorization-server\nsources:\n- https://gemot.dev/.well-known/oauth-authorization-server\n- https://gemot.dev/try/flat-quill-562842\ndescription: Authentication methods as published on Gemot pages\nschemes:\n- type: apiKey\n  name: join_code\n  evidence: The join_code authenticates sandbox access.\n  location: body\ndocs: https://gemot.dev/.well-known/oauth-authorization-server\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/gemot-dev/authentication/gemot-dev-authentication.yml
summary_line: 1 scheme
tags:
- Governance
- Decentralization
- Autonomous Organizations
- Coordination
- Open Protocol
---
