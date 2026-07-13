---
api_key_in: []
api_specs:
- filename: fauna-core-http-api-openapi.yml
  format: yaml
  label: Fauna Core HTTP API
  slug: core-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fauna/refs/heads/main/openapi/fauna-core-http-api-openapi.yml
- filename: fauna-event-streaming-asyncapi.yml
  format: yaml
  label: Fauna Event Streaming API
  slug: event-streaming-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/fauna/refs/heads/main/asyncapi/fauna-event-streaming-asyncapi.yml
- filename: fauna-graphql-api-openapi.yml
  format: yaml
  label: Fauna GraphQL API
  slug: graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fauna/refs/heads/main/openapi/fauna-graphql-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fauna Authentication
name_suffix: Authentication
oauth_flows: []
overview: fauna secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: fauna
provider_slug: fauna
scheme_count: 1
schemes:
- description: Fauna authentication secret passed as a bearer token. Secrets can be keys, tokens, or JWTs from third-party identity providers.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/fauna-core-http-api-openapi.yml
  - openapi/fauna-graphql-api-openapi.yml
  type: http
slug: fauna-authentication
source_filename: fauna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fauna-core-http-api-openapi.yml, openapi/fauna-graphql-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Fauna authentication secret passed as a bearer token. Secrets can be keys, tokens,\n    or JWTs from third-party identity providers.\n  sources:\n  - openapi/fauna-core-http-api-openapi.yml\n  - openapi/fauna-graphql-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fauna/refs/heads/main/authentication/fauna-authentication.yml
summary_line: http · 1 scheme
tags: []
---
