---
anonymous_access: false
api_key_in: []
api_specs:
- filename: machina-gg-forecast-signals-api-openapi.yml
  format: yaml
  label: Machina Sports Forecast Signals API
  slug: machina-gg-forecast-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machina-gg/openapi/machina-gg-forecast-signals-api-openapi.yml
- filename: machina-gg-intelligence-api-openapi.yml
  format: yaml
  label: Machina Sports Intelligence API
  slug: machina-gg-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machina-gg/openapi/machina-gg-intelligence-api-openapi.yml
- filename: machina-gg-markets-api-openapi.yml
  format: yaml
  label: Machina Sports Markets API
  slug: machina-gg-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machina-gg/openapi/machina-gg-markets-api-openapi.yml
- filename: machina-gg-match-context-api-openapi.yml
  format: yaml
  label: Machina Sports Match Context API
  slug: machina-gg-match-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machina-gg/openapi/machina-gg-match-context-api-openapi.yml
- filename: machina-gg-skills-api-openapi.yml
  format: yaml
  label: Machina Sports Skills API
  slug: machina-gg-skills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/machina-gg/openapi/machina-gg-skills-api-openapi.yml
auth_types: []
description: Authentication methods for Machina
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Machina Sports Authentication
name_suffix: Authentication
oauth_flows: []
overview: Machina Sports declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Machina Sports
provider_slug: machina-gg
scheme_count: 1
schemes:
- evidence: API keys are the right choice for CI/CD.
  header: x-api-token
  how_to_obtain: Create an API key in Machina Studio or via the CLI (`machina credentials generate`).
  location: header
  name: API key
  type: apiKey
slug: machina-gg-authentication
source_filename: machina-gg-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.machina.gg/cli/guide/authentication.md
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.machina.gg/cli/guide/authentication.md\nsources:\n- https://docs.machina.gg/cli/guide/authentication.md\n- https://docs.machina.gg/api-reference/create-an-api-key.md\n- https://docs.machina.gg/cli/commands/credentials.md\n- https://docs.machina.gg/quickstart/overview.md\ndescription: Authentication methods for Machina\nschemes:\n- type: apiKey\n  name: API key\n  evidence: API keys are the right choice for CI/CD.\n  location: header\n  header: x-api-token\n  how_to_obtain: Create an API key in Machina Studio or via the CLI (`machina credentials generate`).\nnote: Other methods (browser login, username/password) are CLI-specific and not described as HTTP authentication schemes.\ndocs: https://docs.machina.gg/cli/guide/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/machina-gg/authentication/machina-gg-authentication.yml
summary_line: 1 scheme
tags:
- Sports
- Artificial Intelligence
- Platform
- Sports AI
- Developers
---
