---
api_key_in: []
api_specs:
- filename: fern-api-openapi.yml
  format: yaml
  label: Ask Fern API
  slug: fern-api-ask-fern-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fern-api/refs/heads/main/openapi/fern-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fern Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fern secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fern
provider_slug: fern-api
scheme_count: 1
schemes:
- description: 'Bearer token generated with the `fern token` CLI command and passed as `Authorization: Bearer YOUR_API_TOKEN`. The token is scoped to your Fern organization and does not expire. Used for the hosted Ask Fern REST API and to authenticate the `fern` CLI in CI/CD. The Ask Fern API is available on the Team and Enterprise plans.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fern-api-openapi.yml
  - https://buildwithfern.com/learn/cli-api-reference/cli-reference/commands
  type: http
slug: fern-api-authentication
source_filename: fern-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fern-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token generated with the `fern token` CLI command and passed as\n    `Authorization: Bearer YOUR_API_TOKEN`. The token is scoped to your Fern\n    organization and does not expire. Used for the hosted Ask Fern REST API and\n    to authenticate the `fern` CLI in CI/CD. The Ask Fern API is available on the\n    Team and Enterprise plans.\n  sources:\n  - openapi/fern-api-openapi.yml\n  - https://buildwithfern.com/learn/cli-api-reference/cli-reference/commands\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fern-api/refs/heads/main/authentication/fern-api-authentication.yml
summary_line: http · 1 scheme
tags:
- API Lifecycle
- SDK Generation
- Client Library
- API Documentation
- Developer Tools
- OpenAPI
- CLI
- Open Source
- Developer Experience
---
