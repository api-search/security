---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: chnlsync-com-copper-retirement-api-openapi.yml
  format: yaml
  label: CHNLSYNC Copper Retirement API
  slug: chnlsync-com-copper-retirement-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-copper-retirement-api-openapi.yml
- filename: chnlsync-com-customer-agent-api-openapi.yml
  format: yaml
  label: CHNLSYNC Customer Agent API
  slug: chnlsync-com-customer-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-customer-agent-api-openapi.yml
- filename: chnlsync-com-customer-api-openapi.yml
  format: yaml
  label: CHNLSYNC Customer API
  slug: chnlsync-com-customer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-customer-api-openapi.yml
- filename: chnlsync-com-customer-bills-api-openapi.yml
  format: yaml
  label: CHNLSYNC Customer Bills API
  slug: chnlsync-com-customer-bills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-customer-bills-api-openapi.yml
- filename: chnlsync-com-customer-decisions-api-openapi.yml
  format: yaml
  label: CHNLSYNC Customer Decisions API
  slug: chnlsync-com-customer-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-customer-decisions-api-openapi.yml
- filename: chnlsync-com-customer-helpdesk-api-openapi.yml
  format: yaml
  label: CHNLSYNC Customer Helpdesk API
  slug: chnlsync-com-customer-helpdesk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-customer-helpdesk-api-openapi.yml
- filename: chnlsync-com-customer-intake-api-openapi.yml
  format: yaml
  label: CHNLSYNC Customer Intake API
  slug: chnlsync-com-customer-intake-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-customer-intake-api-openapi.yml
- filename: chnlsync-com-customer-inventory-api-openapi.yml
  format: yaml
  label: CHNLSYNC Customer Inventory API
  slug: chnlsync-com-customer-inventory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-customer-inventory-api-openapi.yml
- filename: chnlsync-com-customer-outcomes-api-openapi.yml
  format: yaml
  label: CHNLSYNC Customer Outcomes API
  slug: chnlsync-com-customer-outcomes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-customer-outcomes-api-openapi.yml
- filename: chnlsync-com-healthz-api-openapi.yml
  format: yaml
  label: CHNLSYNC Healthz API
  slug: chnlsync-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-healthz-api-openapi.yml
- filename: chnlsync-com-inngest-api-openapi.yml
  format: yaml
  label: CHNLSYNC Inngest API
  slug: chnlsync-com-inngest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/chnlsync-com/openapi/chnlsync-com-inngest-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CHNLSYNC Authentication
name_suffix: Authentication
oauth_flows: []
overview: CHNLSYNC secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CHNLSYNC
provider_slug: chnlsync-com
scheme_count: 2
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/chnlsync-com-openapi.yml
  type: http
- in: header
  name: APIKeyHeader
  parameter: X-Agent-API-Key
  sources:
  - openapi/chnlsync-com-openapi.yml
  type: apiKey
slug: chnlsync-com-authentication
source_filename: chnlsync-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource:\n- openapi/chnlsync-com-openapi.yml\n- https://chnlsync.com/llms.txt\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/chnlsync-com-openapi.yml\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Agent-API-Key\n  sources:\n  - openapi/chnlsync-com-openapi.yml\ndocs: https://api.chnlsync.dev/docs\npublic_routes:\n- path: /api/v1/copper-retirement\n  operationId: get_public_copper_retirement_api_v1_copper_retirement_get\n  auth: none\n  evidence: 'Public copper retirement route (no key, CC BY 4.0, cite source_url): https://api.chnlsync.dev/api/v1/copper-retirement?carrier=AT%26T&state=TX'\n  evidence_url: https://chnlsync.com/llms.txt\nnote: The only published API docs are the auto-generated FastAPI Swagger UI at api.chnlsync.dev/docs; no prose authentication guide, key issuance process or OAuth flow is documented.\
  \ Customer routes declare\n  HTTPBearer or the X-Agent-API-Key header in the contract.\n"
source_yaml_url: https://artifacts.apis.io/chnlsync-com/authentication/chnlsync-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Technology Brokerage
- Telecommunications
- Connectivity
- UCaaS
- CCaaS
- Cloud
- Copper Retirement
- Artificial Intelligence
---
