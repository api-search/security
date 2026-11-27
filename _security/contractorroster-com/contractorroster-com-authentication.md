---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: contractorroster-com-billing-api-openapi.yml
  format: yaml
  label: ContractorRoster Billing API
  slug: contractorroster-com-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contractorroster-com/openapi/contractorroster-com-billing-api-openapi.yml
- filename: contractorroster-com-contractors-api-openapi.yml
  format: yaml
  label: ContractorRoster Contractors API
  slug: contractorroster-com-contractors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contractorroster-com/openapi/contractorroster-com-contractors-api-openapi.yml
- filename: contractorroster-com-coverage-api-openapi.yml
  format: yaml
  label: ContractorRoster Coverage API
  slug: contractorroster-com-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contractorroster-com/openapi/contractorroster-com-coverage-api-openapi.yml
- filename: contractorroster-com-reference-api-openapi.yml
  format: yaml
  label: ContractorRoster Reference API
  slug: contractorroster-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/contractorroster-com/openapi/contractorroster-com-reference-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: ContractorRoster Authentication
name_suffix: Authentication
oauth_flows: []
overview: ContractorRoster secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: ContractorRoster
provider_slug: contractorroster-com
scheme_count: 3
schemes:
- description: 'Contractor API key (cr_live_...) may be sent as "X-API-Key: cr_live_..." per the API reference.'
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/contractorroster-com-openapi.yml
  - https://contractorroster.com/api/v1/docs
  type: apiKey
- bearerFormat: cr_live_...
  description: 'Authorization: Bearer cr_live_... (REST /api/v1 and the MCP server at /api/mcp use the same key).'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/contractorroster-com-openapi.yml
  - https://contractorroster.com/api/v1/docs
  type: http
- bearerFormat: re_live_...
  description: Separate Roster Engine REST/npm interface at https://contractorroster.com/api/re/v1 uses X-API-Key re_live_... keys with credits; not covered by the saved OpenAPI. "re_live_ keys use credits at /api/re/v1; cr_live_ keys use a separate prepaid dollar balance at /api/v1 and /api/mcp. Keys and balances are not interchangeable."
  in: header
  name: RosterEngineApiKey
  parameter: X-API-Key
  sources:
  - https://contractorroster.com/developers/guide.md
  type: apiKey
slug: contractorroster-com-authentication
source_filename: contractorroster-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource:\n- https://contractorroster.com/api/v1/docs\n- https://contractorroster.com/developers/guide.md\n- openapi/contractorroster-com-openapi.yml\ndocs: https://contractorroster.com/api/v1/docs\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  key_prefixes:\n  - cr_live_\n  - re_live_\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'Contractor API key (cr_live_...) may be sent as \"X-API-Key: cr_live_...\" per the API reference.'\n  sources:\n  - openapi/contractorroster-com-openapi.yml\n  - https://contractorroster.com/api/v1/docs\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: cr_live_...\n  description: \"Authorization: Bearer cr_live_... (REST /api/v1 and the MCP server at /api/mcp use the same key).\"\n  sources:\n  - openapi/contractorroster-com-openapi.yml\n  - https://contractorroster.com/api/v1/docs\n- name: RosterEngineApiKey\n\
  \  type: apiKey\n  in: header\n  parameter: X-API-Key\n  bearerFormat: re_live_...\n  description: 'Separate Roster Engine REST/npm interface at https://contractorroster.com/api/re/v1 uses X-API-Key re_live_... keys with credits; not covered by the saved OpenAPI. \"re_live_ keys use credits at /api/re/v1; cr_live_ keys use a separate prepaid dollar balance at /api/v1 and /api/mcp. Keys and balances are not interchangeable.\"'\n  sources:\n  - https://contractorroster.com/developers/guide.md\nkey_issuance:\n  contractor_api: Self-serve key emailed via https://contractorroster.com/mcp (\"emailed in under a minute, free lookups immediately, no card\").\n  roster_engine: Created via POST /api/re/v1/keys with an email; returned once with free_credits 0 (documented, not called).\npublic_endpoints:\n- GET /api/v1/coverage\n- GET /api/v1/states\n- GET /api/v1/trades\n- GET /api/re/v1/rosters\n- GET /api/re/v1/notices\nguidance: Keep keys in server-side secrets, never browser code, prompts, URLs\
  \ or logs (developer guide).\n"
source_yaml_url: https://artifacts.apis.io/contractorroster-com/authentication/contractorroster-com-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- Contractors
- Business Data
- Licensing Records
- Lead Generation
- Data Enrichment
- MCP
- Construction
---
