---
api_key_in: []
api_specs:
- filename: swagger-codegen-generation-api-openapi.yml
  format: yaml
  label: Swagger Codegen Generation API
  slug: swagger-codegen-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-generation-api-openapi.yml
- filename: swagger-codegen-languages-api-openapi.yml
  format: yaml
  label: Swagger Codegen Languages API
  slug: swagger-codegen-languages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-languages-api-openapi.yml
- filename: swagger-codegen-options-api-openapi.yml
  format: yaml
  label: Swagger Codegen Options API
  slug: swagger-codegen-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-options-api-openapi.yml
- filename: swagger-codegen-utilities-api-openapi.yml
  format: yaml
  label: Swagger Codegen Utilities API
  slug: swagger-codegen-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/openapi/swagger-codegen-utilities-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Swagger Codegen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swagger Codegen declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Swagger Codegen
provider_slug: swagger-codegen
scheme_count: 0
schemes: []
slug: swagger-codegen-authentication
source_filename: swagger-codegen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: https://generator3.swagger.io/openapi.json\ndocs: https://github.com/swagger-api/swagger-codegen/wiki\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  model: none\n  public: true\nschemes: []\nfindings:\n  - >-\n    Neither published contract declares a securitySchemes / securityDefinitions\n    block. The v3 spec at generator3.swagger.io/openapi.json has no\n    components.securitySchemes; the v2 spec at generator.swagger.io/api/swagger.json\n    has no securityDefinitions.\n  - >-\n    Verified by unauthenticated call: GET https://generator3.swagger.io/api/clients\n    returned 200 with the full language array and no credential of any kind.\n  - >-\n    The service returns permissive CORS (access-control-allow-origin: *) and\n    advertises api_key and Authorization in access-control-allow-headers, but\n    neither is required by any operation and neither is declared in the spec.\n  - >-\n    AuthorizationValue\
  \ in the request schema is NOT authentication for this API.\n    It carries credentials the generator should use when fetching the CALLER's\n    remote OpenAPI definition (specURL) — a passthrough, not a gate.\nevidence:\n  - {url: 'https://generator3.swagger.io/api/clients', http_status: 200, auth_sent: none, fetched: '2026-08-06'}\n  - {url: 'https://generator3.swagger.io/openapi.json', http_status: 200, securitySchemes: absent, fetched: '2026-08-06'}\n  - {url: 'https://generator.swagger.io/api/swagger.json', http_status: 200, securityDefinitions: absent, fetched: '2026-08-06'}\nagent_guidance: >-\n  No credential acquisition step is required. An agent can call every operation\n  anonymously. There is no rate-limit header, no quota, and no account, so an\n  agent must self-throttle — see rate-limits/ and conventions/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swagger-codegen/refs/heads/main/authentication/swagger-codegen-authentication.yml
summary_line: 0 schemes
tags:
- Client Libraries
- Code Generation
- Open Source
- OpenAPI
- SDK
---
