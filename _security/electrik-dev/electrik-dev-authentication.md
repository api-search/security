---
anonymous_access: false
api_key_in: []
api_specs:
- filename: electrik-dev-openapi-generated.yml
  format: yaml
  label: Electrik API
  slug: electrik-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/electrik-dev/openapi/_ae-authored/electrik-dev-openapi-generated.yml
auth_types: []
description: Electrik uses Laravel Sanctum personal access tokens for API authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Electrik Authentication
name_suffix: Authentication
oauth_flows: []
overview: Electrik declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Electrik
provider_slug: electrik-dev
scheme_count: 1
schemes:
- evidence: 'curl -H "Authorization: Bearer <token>" https://your-app.test/api/electrik/me'
  header: Authorization
  how_to_obtain: Users create and revoke tokens from Settings → API tokens in the UI.
  location: header
  name: Bearer token
  type: http-bearer
slug: electrik-dev-authentication
source_filename: electrik-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://electrik.dev/docs/core-concepts/auth-security/
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://electrik.dev/docs/core-concepts/auth-security/\nsources:\n- https://electrik.dev/docs/core-concepts/auth-security/\n- https://electrik.dev/docs/guides/api-tokens/\n- https://electrik.dev/docs/getting-started/introduction/\n- https://electrik.dev/docs/getting-started/quickstart/\ndescription: Electrik uses Laravel Sanctum personal access tokens for API authentication.\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'curl -H \"Authorization: Bearer <token>\" https://your-app.test/api/electrik/me'\n  location: header\n  header: Authorization\n  how_to_obtain: Users create and revoke tokens from Settings → API tokens in the UI.\ndocs: https://electrik.dev/docs/core-concepts/auth-security/\n"
source_yaml_url: https://artifacts.apis.io/electrik-dev/authentication/electrik-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Laravel
- Software-as-a-Service
- Stripe
- Open Source
- PHP
---
