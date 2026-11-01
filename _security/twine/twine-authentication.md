---
anonymous_access: false
api_key_in: []
api_specs:
- filename: twine-openapi-generated.yml
  format: yaml
  label: Twine Integrations API
  slug: twine-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twine/openapi/_ae-authored/twine-openapi-generated.yml
auth_types: []
description: Authentication methods for Twine Public API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Twine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Twine Integrations declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Twine Integrations
provider_slug: twine
scheme_count: 1
schemes:
- evidence: 'The Twine public API uses Bearer token authentication. Send the token in the `Authorization` header with the value `Bearer <token>`:'
  header: Authorization
  how_to_obtain: Generate a long‑lived refresh token in Twine backoffice, then exchange it for short‑lived access tokens via the `/provisioning/refresh-token/begin` and `/provisioning/refresh-token/refresh` endpoints.
  location: header
  name: Bearer token
  type: http-bearer
slug: twine-authentication
source_filename: twine-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.twine.se/api-reference/authentication.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.twine.se/api-reference/authentication.md\nsources:\n- https://docs.twine.se/api-reference/authentication.md\n- https://docs.twine.se/api-reference/systemintegrations/create-credentials-link.md\n- https://docs.twine.se/api-reference/provisioning/refresh-token.md\n- https://docs.twine.se/api-reference/provisioning/begin-refresh-token-process.md\ndescription: Authentication methods for Twine Public API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'The Twine public API uses Bearer token authentication. Send the token in the `Authorization` header with the value `Bearer <token>`:'\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a long‑lived refresh token in Twine backoffice, then exchange it for short‑lived access tokens via the `/provisioning/refresh-token/begin`\n    and `/provisioning/refresh-token/refresh` endpoints.\ndocs:\
  \ https://docs.twine.se/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/twine/authentication/twine-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Human Resources
- Payroll
- Integration
- Nordic
---
