---
anonymous_access: false
api_key_in: []
api_specs:
- filename: forecall-dev-evaluations-api-openapi.yml
  format: yaml
  label: forecall-dev Evaluations API
  slug: forecall-dev-evaluations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecall-dev/openapi/forecall-dev-evaluations-api-openapi.yml
- filename: forecall-dev-me-api-openapi.yml
  format: yaml
  label: forecall-dev Me API
  slug: forecall-dev-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecall-dev/openapi/forecall-dev-me-api-openapi.yml
- filename: forecall-dev-servers-api-openapi.yml
  format: yaml
  label: forecall-dev Servers API
  slug: forecall-dev-servers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forecall-dev/openapi/forecall-dev-servers-api-openapi.yml
auth_types: []
description: Authentication schemes for forecall-dev API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: forecall-dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: forecall-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: forecall-dev
provider_slug: forecall-dev
scheme_count: 1
schemes:
- evidence: 'Send it in every request. `GET /v1/me` answers with the key''s organization and kind:'
  header: Authorization
  how_to_obtain: Create an API key in the dashboard under API keys.
  location: header
  name: Authorization
  type: http-bearer
slug: forecall-dev-authentication
source_filename: forecall-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://forecall.dev/en/docs/api.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://forecall.dev/en/docs/api.md\nsources:\n- https://forecall.dev/en/docs/api.md\n- https://forecall.dev/en/docs/api\n- https://forecall.dev/en/token.md\n- https://forecall.dev/ja/token.md\ndescription: Authentication schemes for forecall-dev API\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Send it in every request. `GET /v1/me` answers with the key''s organization and kind:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the dashboard under API keys.\ndocs: https://forecall.dev/en/docs/api.md\n"
source_yaml_url: https://artifacts.apis.io/forecall-dev/authentication/forecall-dev-authentication.yml
summary_line: 1 scheme
tags:
- Static Linter
- Description Scoring
- Failure Records
---
