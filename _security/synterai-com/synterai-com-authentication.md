---
anonymous_access: false
api_key_in: []
api_specs:
- filename: synterai-com-openapi-generated.yml
  format: yaml
  label: Synter API
  slug: synterai-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synterai-com/openapi/_ae-authored/synterai-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for Synter API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Synter Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synter declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Synter
provider_slug: synterai-com
scheme_count: 1
schemes:
- evidence: 'Browser OAuth (the client sends Authorization: Bearer <OAuth access token>), or X-Synter-Key: syn_… for headless clients'
  header: Authorization
  how_to_obtain: Obtain an OAuth access token via Synter's browser sign‑in flow; the token is sent in the Authorization header as a Bearer token.
  location: header
  name: OAuth
  type: oauth2
slug: synterai-com-authentication
source_filename: synterai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.synterai.com/api/authentication
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.synterai.com/api/authentication\nsources:\n- https://docs.synterai.com/api/authentication\n- https://docs.synterai.com/api/authentication.md\n- https://docs.synterai.com/api/multi-tenant-auth\n- https://docs.synterai.com/api/multi-tenant-auth.md\ndescription: Authentication schemes for Synter API\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: 'Browser OAuth (the client sends Authorization: Bearer <OAuth access token>), or X-Synter-Key: syn_… for headless clients'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain an OAuth access token via Synter's browser sign‑in flow; the token is sent in the Authorization header as a Bearer token.\ndocs: https://docs.synterai.com/api/authentication\nnote: 3 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/synterai-com/authentication/synterai-com-authentication.yml
summary_line: 1 scheme
tags:
- Advertising
- AI
- Marketing
- Automation
- Platform
---
