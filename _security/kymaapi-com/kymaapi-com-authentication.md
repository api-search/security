---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kymaapi-com-audio-api-openapi.yml
  format: yaml
  label: kymaapi-com Audio API
  slug: kymaapi-com-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-audio-api-openapi.yml
- filename: kymaapi-com-auth-api-openapi.yml
  format: yaml
  label: kymaapi-com Auth API
  slug: kymaapi-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-auth-api-openapi.yml
- filename: kymaapi-com-chat-api-openapi.yml
  format: yaml
  label: kymaapi-com Chat API
  slug: kymaapi-com-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-chat-api-openapi.yml
- filename: kymaapi-com-completions-api-openapi.yml
  format: yaml
  label: kymaapi-com Completions API
  slug: kymaapi-com-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-completions-api-openapi.yml
- filename: kymaapi-com-credits-api-openapi.yml
  format: yaml
  label: kymaapi-com Credits API
  slug: kymaapi-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-credits-api-openapi.yml
- filename: kymaapi-com-decisions-api-openapi.yml
  format: yaml
  label: kymaapi-com Decisions API
  slug: kymaapi-com-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-decisions-api-openapi.yml
- filename: kymaapi-com-discovery-api-openapi.yml
  format: yaml
  label: kymaapi-com Discovery API
  slug: kymaapi-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-discovery-api-openapi.yml
- filename: kymaapi-com-embeddings-api-openapi.yml
  format: yaml
  label: kymaapi-com Embeddings API
  slug: kymaapi-com-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-embeddings-api-openapi.yml
- filename: kymaapi-com-images-api-openapi.yml
  format: yaml
  label: kymaapi-com Images API
  slug: kymaapi-com-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-images-api-openapi.yml
- filename: kymaapi-com-models-api-openapi.yml
  format: yaml
  label: kymaapi-com Models API
  slug: kymaapi-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-models-api-openapi.yml
- filename: kymaapi-com-video-api-openapi.yml
  format: yaml
  label: kymaapi-com Video API
  slug: kymaapi-com-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kymaapi-com/openapi/kymaapi-com-video-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kymaapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: kymaapi-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: kymaapi-com
provider_slug: kymaapi-com
scheme_count: 2
schemes:
- description: Bearer token for API access.
  in: header
  name: Authorization
  type: apiKey
- description: Dashboard session token (ks-...).
  in: header
  name: Authorization
  type: apiKey
slug: kymaapi-com-authentication
source_filename: kymaapi-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://docs.kymaapi.com/api-reference/auth-keys.md\nschemes:\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token for API access.\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Dashboard session token (ks-...).\n"
source_yaml_url: https://artifacts.apis.io/kymaapi-com/authentication/kymaapi-com-authentication.yml
summary_line: 2 schemes
tags:
- LLM
- API Gateway
- AI
- Machine Learning
- Developer Tools
---
