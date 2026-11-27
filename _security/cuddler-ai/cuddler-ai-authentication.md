---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cuddler-ai-platform-api-api-openapi.yml
  format: yaml
  label: Cuddler Platform API
  slug: cuddler-ai-platform-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuddler-ai/openapi/cuddler-ai-platform-api-api-openapi.yml
- filename: cuddler-ai-platform-ark-api-openapi.yml
  format: yaml
  label: Cuddler Platform Ark API
  slug: cuddler-ai-platform-ark-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cuddler-ai/openapi/cuddler-ai-platform-ark-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cuddler Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cuddler secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cuddler
provider_slug: cuddler-ai
scheme_count: 1
schemes:
- bearerFormat: cud_sk_live_…
  description: An organization API key issued by Cuddler (cud_sk_live_… spends the organization's prepaid USD balance; cud_sk_test_… can only read the catalog, estimate, and read the balance and usage).
  header: 'Authorization: Bearer $CUDDLER_API_KEY'
  key_prefixes:
    live: cud_sk_live_
    test: cud_sk_test_
  name: PlatformApiKey
  scheme: bearer
  sources:
  - openapi/cuddler-ai-openapi.yml
  - https://platform.cuddler.ai/docs/authentication
  type: http
slug: cuddler-ai-authentication
source_filename: cuddler-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://platform.cuddler.ai/docs/authentication\nsummary:\n  types:\n  - http\nschemes:\n- name: PlatformApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: cud_sk_live_…\n  description: An organization API key issued by Cuddler (cud_sk_live_… spends the organization's prepaid USD balance;\n    cud_sk_test_… can only read the catalog, estimate, and read the balance and usage).\n  sources:\n  - openapi/cuddler-ai-openapi.yml\n  - https://platform.cuddler.ai/docs/authentication\n  key_prefixes:\n    live: cud_sk_live_\n    test: cud_sk_test_\n  header: 'Authorization: Bearer $CUDDLER_API_KEY'\ndocs: https://platform.cuddler.ai/docs/authentication\nderived_from: openapi/cuddler-ai-openapi.yml\nkey_management:\n  owner: organization (not a person)\n  live_prefix: cud_sk_live_\n  test_prefix: cud_sk_test_\n  shown_once: true\n  storage: hash only; a lost key must be revoked and recreated\n  revocation: console (owners, admins,\
  \ developers); a revoked key stops working immediately\n  rotation: create a new key, deploy it, then revoke the old one\nerrors:\n- status: 401\n  code: unauthorized\n- status: 403\n  code: forbidden\n- status: 403\n  code: organization_suspended\n- status: 403\n  code: model_not_enabled\nnotes:\n- Keys belong to the organization, not to a person; every job records api_key_id.\n- Test keys can call GET /v1/models, GET /v1/models/{id}, POST /v1/videos/estimate, POST /v1/images/estimate, GET\n  /v1/balance and GET /v1/usage only; any other call answers 403 forbidden.\n- The full key is shown once at creation; only a hash is stored. Owners, admins and developers create and revoke\n  keys in the console; a revoked key stops working immediately.\n- No OAuth flows are documented, so no scopes artifact applies.\n"
source_yaml_url: https://artifacts.apis.io/cuddler-ai/authentication/cuddler-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Video Generation
- Image Generation
- Interactive Storytelling
- Generative Media
- MCP
---
