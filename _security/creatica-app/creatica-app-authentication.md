---
anonymous_access: false
api_key_in: []
api_specs:
- filename: creatica-app-backgrounds-api-openapi.yml
  format: yaml
  label: Creatica Backgrounds API
  slug: creatica-app-backgrounds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-backgrounds-api-openapi.yml
- filename: creatica-app-generate-api-openapi.yml
  format: yaml
  label: Creatica Generate API
  slug: creatica-app-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-generate-api-openapi.yml
- filename: creatica-app-mcp-api-openapi.yml
  format: yaml
  label: Creatica MCP API
  slug: creatica-app-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-mcp-api-openapi.yml
- filename: creatica-app-palettes-api-openapi.yml
  format: yaml
  label: Creatica Palettes API
  slug: creatica-app-palettes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-palettes-api-openapi.yml
- filename: creatica-app-render-api-openapi.yml
  format: yaml
  label: Creatica Render API
  slug: creatica-app-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-render-api-openapi.yml
- filename: creatica-app-suggest-api-openapi.yml
  format: yaml
  label: Creatica Suggest API
  slug: creatica-app-suggest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/creatica-app/openapi/creatica-app-suggest-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Creatica Authentication
name_suffix: Authentication
oauth_flows: []
overview: Creatica secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Creatica
provider_slug: creatica-app
scheme_count: 1
schemes:
- client_configuration:
    env:
    - CREATICA_API_KEY
    - CREATICA_API_URL
    flags:
    - --api-key
    - --api-url
    - --hosted
    source: '@creatica/cli 0.1.3 dist/cli.js (npm tarball)'
  description: API key. Optional for low-volume anonymous use.
  global_security: '[{bearer: []}, {}] - the empty alternative makes auth optional on every operation'
  key_issuance: 'Keys come from the Creatica dashboard (pricing page: ''grab a key from the dashboard''; Local tier ''Get an API key'').'
  name: bearer
  scheme: bearer
  sources:
  - openapi/creatica-app-openapi.yml
  type: http
slug: creatica-app-authentication
source_filename: creatica-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: openapi/creatica-app-openapi.yml\ndocs: https://creatica.app/pricing\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: API key. Optional for low-volume anonymous use.\n  sources:\n  - openapi/creatica-app-openapi.yml\n  global_security: \"[{bearer: []}, {}] - the empty alternative makes auth optional on every operation\"\n  key_issuance: \"Keys come from the Creatica dashboard (pricing page: 'grab a key from the dashboard'; Local tier 'Get an API key').\"\n  client_configuration:\n    env: [CREATICA_API_KEY, CREATICA_API_URL]\n    flags: [\"--api-key\", \"--api-url\", \"--hosted\"]\n    source: \"@creatica/cli 0.1.3 dist/cli.js (npm tarball)\"\nnote: No dedicated authentication docs page is published; the public GitHub docs (docs/API.md) linked from the site return 404.\n"
source_yaml_url: https://artifacts.apis.io/creatica-app/authentication/creatica-app-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SVG
- Backgrounds
- Design Tools
- Image Generation
- Generative Art
- MCP
- CLI
- Open Source
---
