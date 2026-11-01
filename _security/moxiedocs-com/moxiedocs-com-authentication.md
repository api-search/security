---
anonymous_access: false
api_key_in: []
api_specs:
- filename: moxiedocs-com-check-drift-api-openapi.yml
  format: yaml
  label: moxiedocs-com Check Drift API
  slug: moxiedocs-com-check-drift-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moxiedocs-com/openapi/moxiedocs-com-check-drift-api-openapi.yml
- filename: moxiedocs-com-docs-api-openapi.yml
  format: yaml
  label: moxiedocs-com Docs API
  slug: moxiedocs-com-docs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/moxiedocs-com/openapi/moxiedocs-com-docs-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Moxiedocs Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: moxiedocs-com secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: moxiedocs-com
provider_slug: moxiedocs-com
scheme_count: 1
schemes:
- description: Repository-scoped MCP token with the `context:read` scope, created from the Moxie Docs dashboard (Settings -> MCP tokens) - no sales call required, available on every plan including the free tier.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/moxiedocs-com-openapi.json
  type: http
slug: moxiedocs-com-authentication
source_filename: moxiedocs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/moxiedocs-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Repository-scoped MCP token with the `context:read` scope, created from the Moxie\n    Docs dashboard (Settings -> MCP tokens) - no sales call required, available on every plan\n    including the free tier.\n  sources:\n  - openapi/moxiedocs-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/moxiedocs-com/authentication/moxiedocs-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Documentation
- AI
- GitHub
- Automation
- Developer Tools
---
