---
anonymous_access: true
api_key_in: []
api_specs:
- filename: cleartracedata-com-contract-intelligence-api-openapi.yml
  format: yaml
  label: ClearTrace Contract Intelligence API
  slug: cleartracedata-com-contract-intelligence-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleartracedata-com/openapi/cleartracedata-com-contract-intelligence-api-openapi.yml
- filename: cleartracedata-com-core-data-api-openapi.yml
  format: yaml
  label: ClearTrace Core Data API
  slug: cleartracedata-com-core-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleartracedata-com/openapi/cleartracedata-com-core-data-api-openapi.yml
- filename: cleartracedata-com-execution-benchmarks-api-openapi.yml
  format: yaml
  label: ClearTrace Execution Benchmarks API
  slug: cleartracedata-com-execution-benchmarks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleartracedata-com/openapi/cleartracedata-com-execution-benchmarks-api-openapi.yml
- filename: cleartracedata-com-live-feed-api-openapi.yml
  format: yaml
  label: ClearTrace Live Feed API
  slug: cleartracedata-com-live-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleartracedata-com/openapi/cleartracedata-com-live-feed-api-openapi.yml
- filename: cleartracedata-com-network-status-api-openapi.yml
  format: yaml
  label: ClearTrace Network Status API
  slug: cleartracedata-com-network-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleartracedata-com/openapi/cleartracedata-com-network-status-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ClearTrace Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClearTrace declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ClearTrace
provider_slug: cleartracedata-com
scheme_count: 2
schemes:
- description: 'Authentication: Open. No key required, and no data is gated behind one.'
  name: anonymous
  type: none
- declared_in_openapi: false
  effect: a free key multiplies every rate limit by 10 and changes nothing else
  in: header
  issuance: 'Self-serve and free: POST /api/v1/keys with an email (required) and use_case (optional), or the MCP tool request_api_key. The key is shown once ("we cannot show it to you again").'
  issuance_operation: create_api_key_api_v1_keys_post
  key_format: 'ct_ prefix (example value in docs: ct_your_key_here)'
  name: X-API-Key
  optional: true
  parameter: X-API-Key
  type: apiKey
slug: cleartracedata-com-authentication
source_filename: cleartracedata-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cleartracedata.com/docs/quickstart\ndocs: https://cleartracedata.com/docs/quickstart\nname: ClearTrace authentication\nsummary: >-\n  Open API: no authentication required on any /api/v1 endpoint and no data is gated. An optional free\n  API key, sent as the X-API-Key header, raises rate limits only (x10). The OpenAPI 1.4.0 contract declares\n  no securitySchemes; the header is documented in prose (quickstart, llms.txt, POST /api/v1/keys description).\nrequired: false\nschemes:\n- name: anonymous\n  type: none\n  description: \"Authentication: Open. No key required, and no data is gated behind one.\"\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  optional: true\n  key_format: \"ct_ prefix (example value in docs: ct_your_key_here)\"\n  effect: \"a free key multiplies every rate limit by 10 and changes nothing else\"\n  issuance: >-\n    Self-serve and free: POST /api/v1/keys with an email\
  \ (required) and use_case (optional), or the MCP\n    tool request_api_key. The key is shown once (\"we cannot show it to you again\").\n  issuance_operation: create_api_key_api_v1_keys_post\n  declared_in_openapi: false\nmcp:\n  endpoint: https://cleartracedata.com/mcp\n  auth: \"No OAuth, no account. The X-API-Key header is optional.\"\nobserved:\n  probed: '2026-11-04'\n  url: https://cleartracedata.com/api/v1/gas\n  http_status: 200\n  note: \"an anonymous GET returned 200 with response header x-api-tier: anon\"\n"
source_yaml_url: https://artifacts.apis.io/cleartracedata-com/authentication/cleartracedata-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Blockchain
- DeFi
- Decentralized Exchange
- Analytics
- On-Chain Data
- MEV
- Benchmarks
---
