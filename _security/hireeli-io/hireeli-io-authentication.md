---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hireeli-io-buyer-agent-api-openapi.yml
  format: yaml
  label: Eli Buyer Agent API
  slug: hireeli-io-buyer-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hireeli-io/openapi/hireeli-io-buyer-agent-api-openapi.yml
- filename: hireeli-io-legacy-api-openapi.yml
  format: yaml
  label: Eli Legacy API
  slug: hireeli-io-legacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hireeli-io/openapi/hireeli-io-legacy-api-openapi.yml
- filename: hireeli-io-own-site-execution-api-openapi.yml
  format: yaml
  label: Eli Own-site execution API
  slug: hireeli-io-own-site-execution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hireeli-io/openapi/hireeli-io-own-site-execution-api-openapi.yml
- filename: hireeli-io-public-api-openapi.yml
  format: yaml
  label: Eli Public API
  slug: hireeli-io-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hireeli-io/openapi/hireeli-io-public-api-openapi.yml
- filename: hireeli-io-workspace-reads-api-openapi.yml
  format: yaml
  label: Eli Workspace reads API
  slug: hireeli-io-workspace-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hireeli-io/openapi/hireeli-io-workspace-reads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Eli Authentication
name_suffix: Authentication
oauth_flows: []
overview: Eli secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Eli
provider_slug: hireeli-io
scheme_count: 1
schemes:
- bearerFormat: ELI_API_KEY
  description: A scoped key in the eli_live_<key_id>_<secret> format. The plaintext is shown only when the key is created. The validated key row pins the workspace.
  name: eliApiKey
  scheme: bearer
  sources:
  - openapi/hireeli-io-openapi.json
  type: http
slug: hireeli-io-authentication
source_filename: hireeli-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/hireeli-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: eliApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: ELI_API_KEY\n  description: A scoped key in the eli_live_<key_id>_<secret> format. The plaintext is shown\n    only when the key is created. The validated key row pins the workspace.\n  sources:\n  - openapi/hireeli-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/hireeli-io/authentication/hireeli-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Growth
- SEO
- Automation
- B2B
---
