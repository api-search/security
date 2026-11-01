---
anonymous_access: false
api_key_in: []
api_specs:
- filename: e2a-dev-api-openapi.yml
  format: yaml
  label: e2a API API
  slug: e2a-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/e2a-dev/openapi/_original/e2a-dev-api-openapi.yml
auth_types: []
description: Authentication schemes for e2a API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: E2A Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: e2a-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: e2a-dev
provider_slug: e2a-dev
scheme_count: 1
schemes:
- evidence: 'Both are presented as `Authorization: Bearer <credential>`.'
  header: Authorization
  how_to_obtain: Issued through the e2a dashboard, CLI, or account API and supplied via environment variable `E2A_API_KEY` or config file.
  location: header
  name: API key
  type: http-bearer
slug: e2a-dev-authentication
source_filename: e2a-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://e2a.dev/auth.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://e2a.dev/auth.md\nsources:\n- https://e2a.dev/auth.md\n- https://e2a.dev/setup.md\ndescription: Authentication schemes for e2a API\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Both are presented as `Authorization: Bearer <credential>`.'\n  location: header\n  header: Authorization\n  how_to_obtain: Issued through the e2a dashboard, CLI, or account API and supplied via environment variable `E2A_API_KEY` or config file.\ndocs: https://e2a.dev/auth.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/e2a-dev/authentication/e2a-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Email
- OpenSource
- API
- AI
---
