---
anonymous_access: false
api_key_in: []
api_specs:
- filename: layout-link-openapi-generated.yml
  format: yaml
  label: Layout API
  slug: layout-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layout-link/openapi/_ae-authored/layout-link-openapi-generated.yml
auth_types: []
description: Authentication methods for Layout API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Layout Authentication
name_suffix: Authentication
oauth_flows: []
overview: Layout declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Layout
provider_slug: layout-link
scheme_count: 1
schemes:
- evidence: Send your secret as a bearer token. We read the `Authorization` header and nothing else, so a secret in a query string or a cookie gets ignored rather than quietly working.
  header: Authorization
  location: header
  name: Layout Secret
  type: http-bearer
slug: layout-link-authentication
source_filename: layout-link-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.layout.link/authentication.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.layout.link/authentication.md\nsources:\n- https://docs.layout.link/authentication.md\n- https://docs.layout.link/changelog/oauth-clients-for-your-app.md\n- https://docs.layout.link/changelog/ci-tokens-for-the-cli.md\n- https://docs.layout.link/changelog/a-signing-secret-per-environment.md\ndescription: Authentication methods for Layout API\nschemes:\n- type: http-bearer\n  name: Layout Secret\n  evidence: Send your secret as a bearer token. We read the `Authorization` header and nothing else, so a secret in a query string or a cookie\n    gets ignored rather than quietly working.\n  location: header\n  header: Authorization\ndocs: https://docs.layout.link/authentication.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/layout-link/authentication/layout-link-authentication.yml
summary_line: 1 scheme
tags:
- Food
- Ordering
- Restaurant
- Developers
---
