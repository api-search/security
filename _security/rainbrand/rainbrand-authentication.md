---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: rainbrand-account-api-openapi.yml
  format: yaml
  label: Rainbrand Account API
  slug: rainbrand-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-account-api-openapi.yml
- filename: rainbrand-brands-api-openapi.yml
  format: yaml
  label: Rainbrand Brands API
  slug: rainbrand-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-brands-api-openapi.yml
- filename: rainbrand-images-api-openapi.yml
  format: yaml
  label: Rainbrand Images API
  slug: rainbrand-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-images-api-openapi.yml
- filename: rainbrand-audio-api-openapi.yml
  format: yaml
  label: Rainbrand Audio API
  slug: rainbrand-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-audio-api-openapi.yml
- filename: rainbrand-briefs-api-openapi.yml
  format: yaml
  label: Rainbrand Briefs API
  slug: rainbrand-briefs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-briefs-api-openapi.yml
- filename: rainbrand-feedback-api-openapi.yml
  format: yaml
  label: Rainbrand Feedback API
  slug: rainbrand-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-feedback-api-openapi.yml
- filename: rainbrand-generations-api-openapi.yml
  format: yaml
  label: Rainbrand Generations API
  slug: rainbrand-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-generations-api-openapi.yml
- filename: rainbrand-library-api-openapi.yml
  format: yaml
  label: Rainbrand Library API
  slug: rainbrand-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-library-api-openapi.yml
- filename: rainbrand-models-api-openapi.yml
  format: yaml
  label: Rainbrand Models API
  slug: rainbrand-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-models-api-openapi.yml
- filename: rainbrand-reviews-api-openapi.yml
  format: yaml
  label: Rainbrand Reviews API
  slug: rainbrand-reviews-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-reviews-api-openapi.yml
- filename: rainbrand-uploads-api-openapi.yml
  format: yaml
  label: Rainbrand Uploads API
  slug: rainbrand-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-uploads-api-openapi.yml
- filename: rainbrand-videos-api-openapi.yml
  format: yaml
  label: Rainbrand Videos API
  slug: rainbrand-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/rainbrand/openapi/rainbrand-videos-api-openapi.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Rainbrand Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Rainbrand secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Rainbrand
provider_slug: rainbrand
scheme_count: 3
schemes:
- description: 'Rainbrand API key, for example `x-api-key: bloom_sk_...`.'
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/_original/rainbrand-api-openapi.json
  type: apiKey
- description: Rainbrand API key (`Bearer bloom_sk_...`) or Rainbrand OAuth access token.
  name: bearer
  scheme: bearer
  sources:
  - openapi/_original/rainbrand-api-openapi.json
  type: http
- description: App-integration OAuth (not declared in the OpenAPI securitySchemes; documented in docs/api/authentication with RFC 8414 metadata at /.well-known/oauth-authorization-server).
  flows:
  - authorizationUrl: https://www.rainbrand.com/api/auth/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token
  - flow: refreshToken
    tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token
  issuer: https://www.rainbrand.com/api/auth
  name: Rainbrand OAuth
  registration: https://www.rainbrand.com/api/auth/oauth2/register
  scopes: scopes/rainbrand-scopes.yml
  sources:
  - https://docs.rainbrand.com/authentication
  - well-known/rainbrand-oauth-authorization-server.json
  type: oauth2
slug: rainbrand-authentication
source_filename: rainbrand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/_original/rainbrand-api-openapi.json\ndocs: https://docs.rainbrand.com/authentication\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - refreshToken\nnotes: >-\n  Every request needs a Rainbrand API key (bloom_sk_...) or a Rainbrand OAuth access\n  token. The key is accepted in either header; x-api-key wins when both are\n  present. OAuth tokens resolve to the same user identity as an API key (same\n  access to brands, images, credits, plan gates, workspaces). Public clients\n  use Authorization Code + PKCE S256 with dynamic client registration and no\n  client_secret; wildcard redirect URIs are not supported. Keys are generated\n  at https://www.rainbrand.com/settings#api-keys.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'Rainbrand API key, for example `x-api-key: bloom_sk_...`.'\n\
  \  sources:\n  - openapi/_original/rainbrand-api-openapi.json\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Rainbrand API key (`Bearer bloom_sk_...`) or Rainbrand OAuth access token.\n  sources:\n  - openapi/_original/rainbrand-api-openapi.json\n- name: Rainbrand OAuth\n  type: oauth2\n  description: >-\n    App-integration OAuth (not declared in the OpenAPI securitySchemes;\n    documented in docs/api/authentication with RFC 8414 metadata at\n    /.well-known/oauth-authorization-server).\n  issuer: https://www.rainbrand.com/api/auth\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.rainbrand.com/api/auth/oauth2/authorize\n    tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token\n    pkce: S256\n  - flow: clientCredentials\n    tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token\n  - flow: refreshToken\n    tokenUrl: https://www.rainbrand.com/api/auth/oauth2/token\n  registration: https://www.rainbrand.com/api/auth/oauth2/register\n\
  \  scopes: scopes/rainbrand-scopes.yml\n  sources:\n  - https://docs.rainbrand.com/authentication\n  - well-known/rainbrand-oauth-authorization-server.json\n"
source_yaml_url: https://artifacts.apis.io/rainbrand/authentication/rainbrand-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Company
- Brand Management
- Image Generation
- Artificial Intelligence
- Agents
- MCP
- Marketing
- Creative
---
