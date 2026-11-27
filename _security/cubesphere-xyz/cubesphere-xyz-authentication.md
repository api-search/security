---
anonymous_access: true
api_key_in: []
api_specs:
- filename: cubesphere-xyz-companies-api-openapi.yml
  format: yaml
  label: Cubesphere Companies API
  slug: cubesphere-xyz-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cubesphere-xyz/openapi/cubesphere-xyz-companies-api-openapi.yml
- filename: cubesphere-xyz-events-api-openapi.yml
  format: yaml
  label: Cubesphere Events API
  slug: cubesphere-xyz-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cubesphere-xyz/openapi/cubesphere-xyz-events-api-openapi.yml
- filename: cubesphere-xyz-health-api-openapi.yml
  format: yaml
  label: Cubesphere Health API
  slug: cubesphere-xyz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cubesphere-xyz/openapi/cubesphere-xyz-health-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cubesphere Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cubesphere declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cubesphere
provider_slug: cubesphere-xyz
scheme_count: 2
schemes:
- declared_in_spec: false
  description_text: '`X-API-Key` 헤더 없음 = free 티어(기본값). 유효한 키 = 24시간 게이트 우회 + tenant 가 소유한 basic/pro 한도. 키가 있는데 무효·폐기면 401(조용히 free 로 강등하지 않는다).'
  in: header
  invalid_key_status: 401
  name: X-API-Key
  parameter: X-API-Key
  required: false
  type: apiKey
- description: No header = free tier (24-hour-delayed data, per-IP limits).
  name: anonymous
  type: none
slug: cubesphere-xyz-authentication
source_filename: cubesphere-xyz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://api.cubesphere.xyz/openapi.json\ndocs: https://api.cubesphere.xyz/docs\nnote: The OpenAPI declares no components.securitySchemes; the scheme below is documented only in prose in info.description (### 인증). The key is optional — no key means the free tier.\nschemes:\n- name: X-API-Key\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  required: false\n  description_text: '`X-API-Key` 헤더 없음 = free 티어(기본값). 유효한 키 = 24시간 게이트 우회 + tenant 가 소유한 basic/pro 한도. 키가 있는데 무효·폐기면 401(조용히 free 로 강등하지 않는다).'\n  invalid_key_status: 401\n  declared_in_spec: false\n- name: anonymous\n  type: none\n  description: No header = free tier (24-hour-delayed data, per-IP limits).\n"
source_yaml_url: https://artifacts.apis.io/cubesphere-xyz/authentication/cubesphere-xyz-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Financial Data
- SEC Filings
- Insider Trading
- Cryptocurrency
- Market Intelligence
- MCP
---
