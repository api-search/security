---
api_key_in:
- header
api_specs:
- filename: appsmax-rest-api-v1-access-api-openapi.yml
  format: yaml
  label: AppsMax Access API
  slug: appsmax-rest-api-v1-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-access-api-openapi.yml
- filename: appsmax-rest-api-v1-applications-api-openapi.yml
  format: yaml
  label: AppsMax Applications API
  slug: appsmax-rest-api-v1-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-applications-api-openapi.yml
- filename: appsmax-rest-api-v1-bots-api-openapi.yml
  format: yaml
  label: AppsMax Bots API
  slug: appsmax-rest-api-v1-bots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-bots-api-openapi.yml
- filename: appsmax-rest-api-v1-campaigns-api-openapi.yml
  format: yaml
  label: AppsMax Campaigns API
  slug: appsmax-rest-api-v1-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-campaigns-api-openapi.yml
- filename: appsmax-rest-api-v1-funnels-api-openapi.yml
  format: yaml
  label: AppsMax Funnels API
  slug: appsmax-rest-api-v1-funnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-funnels-api-openapi.yml
- filename: appsmax-rest-api-v1-interactive-menu-api-openapi.yml
  format: yaml
  label: AppsMax Interactive menu API
  slug: appsmax-rest-api-v1-interactive-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-interactive-menu-api-openapi.yml
- filename: appsmax-rest-api-v1-miniapps-api-openapi.yml
  format: yaml
  label: AppsMax Miniapps API
  slug: appsmax-rest-api-v1-miniapps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-miniapps-api-openapi.yml
- filename: appsmax-rest-api-v1-organizations-api-openapi.yml
  format: yaml
  label: AppsMax Organizations API
  slug: appsmax-rest-api-v1-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-organizations-api-openapi.yml
- filename: appsmax-rest-api-v1-subscribers-api-openapi.yml
  format: yaml
  label: AppsMax Subscribers API
  slug: appsmax-rest-api-v1-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/openapi/appsmax-rest-api-v1-subscribers-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Appsmax Rest Api V1 Authentication
name_suffix: Authentication
oauth_flows: []
overview: AppsMax secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AppsMax
provider_slug: appsmax-rest-api-v1
scheme_count: 2
schemes:
- bearerFormat: AppsMax API token
  description: 'Рекомендуемый вариант: Authorization: Bearer YOUR_API_TOKEN'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/appsmax-rest-api-v1-openapi-original.json
  type: http
- description: Fallback для клиентов без Bearer auth. Не передавайте токен в URL.
  in: header
  name: apiTokenHeader
  parameter: X-Api-Token
  sources:
  - openapi/appsmax-rest-api-v1-openapi-original.json
  type: apiKey
slug: appsmax-rest-api-v1-authentication
source_filename: appsmax-rest-api-v1-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: derived\nsource: openapi/appsmax-rest-api-v1-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: AppsMax API token\n  description: 'Рекомендуемый вариант: Authorization: Bearer YOUR_API_TOKEN'\n  sources:\n  - openapi/appsmax-rest-api-v1-openapi-original.json\n- name: apiTokenHeader\n  type: apiKey\n  in: header\n  parameter: X-Api-Token\n  description: Fallback для клиентов без Bearer auth. Не передавайте токен в URL.\n  sources:\n  - openapi/appsmax-rest-api-v1-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/appsmax-rest-api-v1/refs/heads/main/authentication/appsmax-rest-api-v1-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- SaaS
- Messaging
- Business Automation
- Chatbots
- Mini Apps
- Customer Requests
- Workflow Automation
- MAX
- Telegram
- Russian Language
---
