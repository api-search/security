---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mellow-world-openapi-generated.yml
  format: yaml
  label: mellow-world API
  slug: mellow-world-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mellow-world/openapi/_ae-authored/mellow-world-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mellow World Authentication
name_suffix: Authentication
oauth_flows: []
overview: mellow-world declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mellow-world
provider_slug: mellow-world
scheme_count: 1
schemes:
- evidence: '"bearer_methods_supported":["header"]"'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: mellow-world-authentication
source_filename: mellow-world-authentication.yml
source_heading: Authentication Profile
source_url: https://www.mellow.world/api/hub/v1/platforms
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.mellow.world/api/hub/v1/platforms\nsources:\n- https://www.mellow.world/api/hub/v1/platforms\n- https://www.mellow.world/.well-known/oauth-protected-resource\n- https://www.mellow.world/hub/prompts/chatgpt-dots-setup-checklist\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '\"bearer_methods_supported\":[\"header\"]\"'\n  location: header\n  header: Authorization\ndocs: https://www.mellow.world/api/hub/v1/platforms\n"
source_yaml_url: https://artifacts.apis.io/mellow-world/authentication/mellow-world-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Social Media
- Marketing
- Scheduling
- Content Creation
- SaaS
---
