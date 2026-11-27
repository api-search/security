---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nexip-ru-billing-api-openapi.yml
  format: yaml
  label: NexIP Billing API
  slug: nexip-ru-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-billing-api-openapi.yml
- filename: nexip-ru-comparisons-api-openapi.yml
  format: yaml
  label: NexIP Comparisons API
  slug: nexip-ru-comparisons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-comparisons-api-openapi.yml
- filename: nexip-ru-monitoring-api-openapi.yml
  format: yaml
  label: NexIP Monitoring API
  slug: nexip-ru-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-monitoring-api-openapi.yml
- filename: nexip-ru-notifications-api-openapi.yml
  format: yaml
  label: NexIP Notifications API
  slug: nexip-ru-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-notifications-api-openapi.yml
- filename: nexip-ru-public-entities-api-openapi.yml
  format: yaml
  label: NexIP Public Entities API
  slug: nexip-ru-public-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-public-entities-api-openapi.yml
- filename: nexip-ru-reports-api-openapi.yml
  format: yaml
  label: NexIP Reports API
  slug: nexip-ru-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-reports-api-openapi.yml
- filename: nexip-ru-seo-audit-api-openapi.yml
  format: yaml
  label: NexIP SEO Audit API
  slug: nexip-ru-seo-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-seo-audit-api-openapi.yml
- filename: nexip-ru-system-api-openapi.yml
  format: yaml
  label: NexIP System API
  slug: nexip-ru-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-system-api-openapi.yml
- filename: nexip-ru-tools-api-openapi.yml
  format: yaml
  label: NexIP Tools API
  slug: nexip-ru-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nexip-ru/openapi/nexip-ru-tools-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: NexIP Authentication
name_suffix: Authentication
oauth_flows: []
overview: NexIP secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NexIP
provider_slug: nexip-ru
scheme_count: 2
schemes:
- bearerFormat: NexIP API Key
  description: 'Предпочтительный вариант: Authorization: Bearer nxp_live_...'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/nexip-ru-openapi.json
  type: http
- description: Совместимый вариант передачи API-ключа.
  in: header
  name: ApiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/nexip-ru-openapi.json
  type: apiKey
slug: nexip-ru-authentication
source_filename: nexip-ru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nexip-ru-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: NexIP API Key\n  description: 'Предпочтительный вариант: Authorization: Bearer nxp_live_...'\n  sources:\n  - openapi/nexip-ru-openapi.json\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Совместимый вариант передачи API-ключа.\n  sources:\n  - openapi/nexip-ru-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nexip-ru/authentication/nexip-ru-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
---
