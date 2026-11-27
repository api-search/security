---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gnosem-dev-auth-api-openapi.yml
  format: yaml
  label: Gnosem Auth API
  slug: gnosem-dev-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosem-dev/openapi/gnosem-dev-auth-api-openapi.yml
- filename: gnosem-dev-demo-api-openapi.yml
  format: yaml
  label: Gnosem Demo API
  slug: gnosem-dev-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosem-dev/openapi/gnosem-dev-demo-api-openapi.yml
- filename: gnosem-dev-export-api-openapi.yml
  format: yaml
  label: Gnosem Export API
  slug: gnosem-dev-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosem-dev/openapi/gnosem-dev-export-api-openapi.yml
- filename: gnosem-dev-health-api-openapi.yml
  format: yaml
  label: Gnosem Health API
  slug: gnosem-dev-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosem-dev/openapi/gnosem-dev-health-api-openapi.yml
- filename: gnosem-dev-keys-api-openapi.yml
  format: yaml
  label: Gnosem Keys API
  slug: gnosem-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosem-dev/openapi/gnosem-dev-keys-api-openapi.yml
- filename: gnosem-dev-mcp-api-openapi.yml
  format: yaml
  label: Gnosem MCP API
  slug: gnosem-dev-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosem-dev/openapi/gnosem-dev-mcp-api-openapi.yml
- filename: gnosem-dev-me-api-openapi.yml
  format: yaml
  label: Gnosem Me API
  slug: gnosem-dev-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosem-dev/openapi/gnosem-dev-me-api-openapi.yml
- filename: gnosem-dev-signup-api-openapi.yml
  format: yaml
  label: Gnosem Signup API
  slug: gnosem-dev-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosem-dev/openapi/gnosem-dev-signup-api-openapi.yml
- filename: gnosem-dev-stripe-api-openapi.yml
  format: yaml
  label: Gnosem Stripe API
  slug: gnosem-dev-stripe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosem-dev/openapi/gnosem-dev-stripe-api-openapi.yml
- filename: gnosem-dev-upgrade-api-openapi.yml
  format: yaml
  label: Gnosem Upgrade API
  slug: gnosem-dev-upgrade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gnosem-dev/openapi/gnosem-dev-upgrade-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Gnosem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gnosem secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gnosem
provider_slug: gnosem-dev
scheme_count: 1
schemes:
- bearerFormat: gn_[a-f0-9]{32}
  description: 'Every user gets an API key on signup formatted as `gn_` + 32 hex characters. Pass as `Authorization: Bearer <key>` on every authenticated request.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gnosem-dev-openapi.json
  type: http
slug: gnosem-dev-authentication
source_filename: gnosem-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/gnosem-dev-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: gn_[a-f0-9]{32}\n  description: 'Every user gets an API key on signup formatted as `gn_` + 32 hex characters.\n    Pass as `Authorization: Bearer <key>` on every authenticated request.'\n  sources:\n  - openapi/gnosem-dev-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/gnosem-dev/authentication/gnosem-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Memory
- MCP
- Cross-vendor
- Cloud
---
