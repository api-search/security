---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tohuman-openapi-generated.yml
  format: yaml
  label: ToHuman API
  slug: tohuman-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tohuman/refs/heads/main/openapi/_ae-authored/tohuman-openapi-generated.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Tohuman Authentication
name_suffix: Authentication
oauth_flows: []
overview: ToHuman declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ToHuman
provider_slug: tohuman
scheme_count: 1
schemes:
- evidence: Every ToHuman API endpoint requires that token as a bearer credential in the Authorization header — there is no other auth scheme, and no query-parameter fallback.
  header: Authorization
  how_to_obtain: Sign in to your ToHuman dashboard and create a new API token.
  location: header
  name: Bearer
  type: http-bearer
slug: tohuman-authentication
source_filename: tohuman-authentication.yml
source_heading: Authentication Profile
source_url: https://tohuman.io/docs/quickstart#authentication
source_yaml: "generated: '2026-09-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://tohuman.io/docs/quickstart#authentication\nsources:\n- https://tohuman.io/docs/quickstart#authentication\n- https://tohuman.io/docs/quickstart\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every ToHuman API endpoint requires that token as a bearer credential in the Authorization header — there is no other auth scheme,\n    and no query-parameter fallback.\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in to your ToHuman dashboard and create a new API token.\ndocs: https://tohuman.io/docs/quickstart#authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tohuman/refs/heads/main/authentication/tohuman-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Text-Humanization
- Content-Generation
- Marketing
- SaaS
---
