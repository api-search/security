---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: boltena-com-default-api-openapi.yml
  format: yaml
  label: 볼테나 기본 API
  slug: boltena-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boltena-com/openapi/boltena-com-default-api-openapi.yml
- filename: boltena-com-eqp-api-openapi.yml
  format: yaml
  label: 볼테나 EQP 모듈 필요 API
  slug: boltena-com-eqp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boltena-com/openapi/boltena-com-eqp-api-openapi.yml
- filename: boltena-com-hr-api-openapi.yml
  format: yaml
  label: 볼테나 HR 모듈 필요 API
  slug: boltena-com-hr-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/boltena-com/openapi/boltena-com-hr-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: 볼테나 Authentication
name_suffix: Authentication
oauth_flows: []
overview: 볼테나 secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: 볼테나
provider_slug: boltena-com
scheme_count: 1
schemes:
- description: 제품의 시스템 > API 키 관리에서 발급합니다. 키에 회사 정보가 담겨 있어 회사코드를 따로 보내지 않습니다.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/boltena-com-openapi.json
  type: apiKey
slug: boltena-com-authentication
source_filename: boltena-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/boltena-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 제품의 시스템 > API 키 관리에서 발급합니다. 키에 회사 정보가 담겨 있어 회사코드를 따로 보내지 않습니다.\n  sources:\n  - openapi/boltena-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/boltena-com/authentication/boltena-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ERP
- Human Resources
- MES
- Business Intelligence
---
