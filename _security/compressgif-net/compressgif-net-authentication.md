---
anonymous_access: false
api_key_in: []
api_specs:
- filename: compressgif-net-compressions-api-openapi.yml
  format: yaml
  label: CompressGIF Compressions API
  slug: compressgif-net-compressions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compressgif-net/openapi/compressgif-net-compressions-api-openapi.yml
- filename: compressgif-net-usage-api-openapi.yml
  format: yaml
  label: CompressGIF Usage API
  slug: compressgif-net-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/compressgif-net/openapi/compressgif-net-usage-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CompressGIF Authentication
name_suffix: Authentication
oauth_flows: []
overview: CompressGIF declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CompressGIF
provider_slug: compressgif-net
scheme_count: 2
schemes:
- bearerFormat: API key
  description: Send Authorization Bearer YOUR_API_KEY on create, status and usage requests. The documented key examples use the cg_live_ prefix.
  header: Authorization
  name: bearerKey
  scheme: bearer
  type: http
- description: The API also accepts the x-api-key header.
  header: x-api-key
  in: header
  name: apiKey
  type: apiKey
slug: compressgif-net-authentication
source_filename: compressgif-net-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://compressgif.net/docs\ndocs: https://compressgif.net/docs\nschemes:\n- name: bearerKey\n  type: http\n  scheme: bearer\n  bearerFormat: API key\n  header: Authorization\n  description: Send Authorization Bearer YOUR_API_KEY on create, status and usage requests. The documented key examples use the cg_live_ prefix.\n- name: apiKey\n  type: apiKey\n  in: header\n  header: x-api-key\n  description: The API also accepts the x-api-key header.\nkey_management:\n  issuance: Create an API key from account settings (/settings/apikeys) after activating free API access or subscribing to Developer.\n  sharing: All keys belonging to one account share allowances and limits.\n  revocation: If a key is exposed, revoke it in API key settings and create a replacement.\n  notes: Account sign-in cookies are not a replacement for an API key. MCP at /api/mcp uses the same API key as REST.\nfree_access_activation: Sign in with Google using\
  \ a verified @gmail.com address and pass Turnstile to activate free API access.\n"
source_yaml_url: https://artifacts.apis.io/compressgif-net/authentication/compressgif-net-authentication.yml
summary_line: 2 schemes
tags:
- Company
- GIF
- Image Compression
- Image Processing
- Animation
- Media
- MCP
- REST API
---
