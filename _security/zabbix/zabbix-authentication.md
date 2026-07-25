---
api_key_in:
- header
api_specs:
- filename: zabbix-actions-api-openapi.yml
  format: yaml
  label: Zabbix Actions API
  slug: zabbix-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-actions-api-openapi.yml
- filename: zabbix-authentication-api-openapi.yml
  format: yaml
  label: Zabbix Authentication API
  slug: zabbix-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-authentication-api-openapi.yml
- filename: zabbix-events-api-openapi.yml
  format: yaml
  label: Zabbix Events API
  slug: zabbix-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-events-api-openapi.yml
- filename: zabbix-history-api-openapi.yml
  format: yaml
  label: Zabbix History API
  slug: zabbix-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-history-api-openapi.yml
- filename: zabbix-host-groups-api-openapi.yml
  format: yaml
  label: Zabbix Host Groups API
  slug: zabbix-host-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-host-groups-api-openapi.yml
- filename: zabbix-hosts-api-openapi.yml
  format: yaml
  label: Zabbix Hosts API
  slug: zabbix-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-hosts-api-openapi.yml
- filename: zabbix-items-api-openapi.yml
  format: yaml
  label: Zabbix Items API
  slug: zabbix-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-items-api-openapi.yml
- filename: zabbix-problems-api-openapi.yml
  format: yaml
  label: Zabbix Problems API
  slug: zabbix-problems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-problems-api-openapi.yml
- filename: zabbix-triggers-api-openapi.yml
  format: yaml
  label: Zabbix Triggers API
  slug: zabbix-triggers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-triggers-api-openapi.yml
- filename: zabbix-users-api-openapi.yml
  format: yaml
  label: Zabbix Users API
  slug: zabbix-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zabbix/refs/heads/main/openapi/zabbix-users-api-openapi.yml
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
