---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: ludo-ai-audio-api-openapi.yml
  format: yaml
  label: Ludo.ai Audio API
  slug: ludo-ai-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-audio-api-openapi.yml
- filename: ludo-ai-images-api-openapi.yml
  format: yaml
  label: Ludo.ai Images API
  slug: ludo-ai-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-images-api-openapi.yml
- filename: ludo-ai-spritesheets-api-openapi.yml
  format: yaml
  label: Ludo.ai Spritesheets API
  slug: ludo-ai-spritesheets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-spritesheets-api-openapi.yml
- filename: ludo-ai-videos-api-openapi.yml
  format: yaml
  label: Ludo.ai Videos API
  slug: ludo-ai-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-videos-api-openapi.yml
- filename: ludo-ai-3d-models-api-openapi.yml
  format: yaml
  label: Ludo.ai 3D Models API
  slug: ludo-ai-3d-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-3d-models-api-openapi.yml
- filename: ludo-ai-jobs-api-openapi.yml
  format: yaml
  label: Ludo.ai Jobs API
  slug: ludo-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-jobs-api-openapi.yml
- filename: ludo-ai-generations-api-openapi.yml
  format: yaml
  label: Ludo.ai Generations API
  slug: ludo-ai-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-generations-api-openapi.yml
- filename: ludo-ai-files-api-openapi.yml
  format: yaml
  label: Ludo.ai Files API
  slug: ludo-ai-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-files-api-openapi.yml
- filename: ludo-ai-documentation-api-openapi.yml
  format: yaml
  label: Ludo.ai Documentation API
  slug: ludo-ai-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-documentation-api-openapi.yml
- filename: ludo-ai-account-api-openapi.yml
  format: yaml
  label: Ludo.ai Account API
  slug: ludo-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-account-api-openapi.yml
- filename: ludo-ai-authentication-api-openapi.yml
  format: yaml
  label: Ludo.ai Authentication API
  slug: ludo-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-authentication-api-openapi.yml
- filename: ludo-ai-pricing-api-openapi.yml
  format: yaml
  label: Ludo.ai Pricing API
  slug: ludo-ai-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ludo-ai/openapi/ludo-ai-pricing-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ludo.ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ludo.ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Ludo.ai
provider_slug: ludo-ai
scheme_count: 1
schemes:
- description: Every request carries the `Authorization` header with the literal value `ApiKey <YOUR_API_KEY>`. Keys are created in the web app at app.ludo.ai (API Keys in the sidebar or user menu); each key is shown only once at creation time. A separate CLI key is created and revoked by `ludo login` / `ludo logout`. GET /auth/validate-api-key returns 200 for a valid key and 403 for an invalid one. API, MCP and CLI access is included on the Pro and Studio plans.
  in: header
  name: ApiKey
  parameter: Authorization
  scheme_format: ApiKey <KEY>
  sources:
  - https://api.ludo.ai/api-documentation/openapi.json
  - https://ludo.ai/developers/api
  - https://ludo.ai/developers/mcp
  type: apiKey
slug: ludo-ai-authentication
source_filename: ludo-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: searched\nsource: https://api.ludo.ai/api-documentation/openapi.json\ndocs: https://ludo.ai/developers/api\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - header\nschemes:\n  - name: ApiKey\n    type: apiKey\n    in: header\n    parameter: Authorization\n    scheme_format: 'ApiKey <KEY>'\n    description: >-\n      Every request carries the `Authorization` header with the literal value\n      `ApiKey <YOUR_API_KEY>`. Keys are created in the web app at\n      app.ludo.ai (API Keys in the sidebar or user menu); each key is shown\n      only once at creation time. A separate CLI key is created and revoked by\n      `ludo login` / `ludo logout`. GET /auth/validate-api-key returns 200 for a\n      valid key and 403 for an invalid one. API, MCP and CLI access is included\n      on the Pro and Studio plans.\n    sources:\n      - https://api.ludo.ai/api-documentation/openapi.json\n      - https://ludo.ai/developers/api\n      - https://ludo.ai/developers/mcp\n\
  notes:\n  - The OpenAPI 3.0 spec declares one security scheme named `ApiKey` whose\n    `name` field is `Authorization` (NOT \"Authentication\"); the correct header\n    key is `Authorization`.\n  - The spec version is 0.9.10 and the base URL is https://api.ludo.ai/api.\n  - No OAuth 2 / OpenID Connect / mTLS schemes are declared.\n"
source_yaml_url: https://artifacts.apis.io/ludo-ai/authentication/ludo-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Asset Generation
- Game Design
- Game Development
- Game Asset Generation
- AI Art
- Sprite Sheets
- Model Context Protocol
- CLI
---
