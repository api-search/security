---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: createmod-com-analytics-api-openapi.yml
  format: yaml
  label: CreateMod.com Analytics API
  slug: createmod-com-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createmod-com/openapi/createmod-com-analytics-api-openapi.yml
- filename: createmod-com-mod-integration-api-openapi.yml
  format: yaml
  label: CreateMod.com Mod Integration API
  slug: createmod-com-mod-integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createmod-com/openapi/createmod-com-mod-integration-api-openapi.yml
- filename: createmod-com-schematics-api-openapi.yml
  format: yaml
  label: CreateMod.com Schematics API
  slug: createmod-com-schematics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/createmod-com/openapi/createmod-com-schematics-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: CreateMod.com Authentication
name_suffix: Authentication
oauth_flows: []
overview: CreateMod.com secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CreateMod.com
provider_slug: createmod-com
scheme_count: 3
schemes:
- description: API key passed via X-API-Key header. Generate at /settings/api-keys.
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/createmod-com-openapi.yml
  type: apiKey
- description: API key passed as a query parameter (less secure, use header when possible).
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/createmod-com-openapi.yml
  type: apiKey
- description: 'HMAC-SHA256 authentication via X-Mod-Message and X-Mod-Signature headers. Message format: timestamp:modversion:mcusername:identifier. The signature is HMAC-SHA256(message, shared_secret) hex-encoded. Timestamps must be within 5 minutes.'
  name: HMACSignature
  scheme: bearer
  sources:
  - openapi/createmod-com-openapi.yml
  type: http
slug: createmod-com-authentication
source_filename: createmod-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://createmod.com/api\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key passed via X-API-Key header. Generate at /settings/api-keys.\n  sources:\n  - openapi/createmod-com-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: API key passed as a query parameter (less secure, use header when possible).\n  sources:\n  - openapi/createmod-com-openapi.yml\n- name: HMACSignature\n  type: http\n  scheme: bearer\n  description: 'HMAC-SHA256 authentication via X-Mod-Message and X-Mod-Signature headers.\n    Message format: timestamp:modversion:mcusername:identifier. The signature is HMAC-SHA256(message,\n    shared_secret) hex-encoded. Timestamps must be within 5 minutes.'\n  sources:\n  - openapi/createmod-com-openapi.yml\ndocs: https://createmod.com/api\n\
  docs_notes:\n- All API requests require an API key. Pass it via the X-API-Key header. Keys are\n  scoped to your account and inherit your user-level rate limits.\n- Generate API keys from your account settings . Keys are shown once at creation,\n  store them securely. Never embed keys in client-side code.\nkey_management:\n  url: https://createmod.com/settings/api-keys\n  shown_once: true\nnote: Spec types HMACSignature as http/bearer, but its description says the signature\n  travels in X-Mod-Message and X-Mod-Signature headers (HMAC-SHA256, 5-minute timestamp\n  window); used only by POST /api/mod/download (modDownload). GET /api/schematics/changes\n  is documented in the spec as public (no API key).\n"
source_yaml_url: https://artifacts.apis.io/createmod-com/authentication/createmod-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Minecraft
- Gaming
- Schematics
- Create Mod
- Community
- User Generated Content
- REST API
---
