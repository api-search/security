---
api_key_in:
- header
api_specs:
- filename: zabbix-openapi.yml
  format: yaml
  label: Zabbix API
  slug: zabbix-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zabbix Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zabbix secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zabbix
provider_slug: zabbix
scheme_count: 1
schemes:
- description: Zabbix API token obtained via user.login. Pass as "Bearer {token}" in the Authorization header (Zabbix 5.4+), or in the auth field of the JSON-RPC request body.
  in: header
  name: ApiToken
  parameter: Authorization
  sources:
  - openapi/zabbix-openapi.yml
  type: apiKey
slug: zabbix-authentication
source_filename: zabbix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zabbix-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Zabbix API token obtained via user.login. Pass as \"Bearer {token}\" in the Authorization\n    header (Zabbix 5.4+), or in the auth field of the JSON-RPC request body.\n  sources:\n  - openapi/zabbix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/authentication/zabbix-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Monitoring
- Infrastructure
- Networks
- Alerting
- Open Source
- Observability
---
