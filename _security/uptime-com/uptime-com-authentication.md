---
api_key_in:
- header
api_specs:
- filename: uptime-com-checks-api-openapi.yml
  format: yaml
  label: Uptime.com Checks API
  slug: uptime-com-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-checks-api-openapi.yml
- filename: uptime-com-contacts-api-openapi.yml
  format: yaml
  label: Uptime.com Contacts API
  slug: uptime-com-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-contacts-api-openapi.yml
- filename: uptime-com-integrations-api-openapi.yml
  format: yaml
  label: Uptime.com Integrations API
  slug: uptime-com-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-integrations-api-openapi.yml
- filename: uptime-com-outages-api-openapi.yml
  format: yaml
  label: Uptime.com Outages API
  slug: uptime-com-outages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-outages-api-openapi.yml
- filename: uptime-com-sla-reports-api-openapi.yml
  format: yaml
  label: Uptime.com SLA Reports API
  slug: uptime-com-sla-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-sla-reports-api-openapi.yml
- filename: uptime-com-status-pages-api-openapi.yml
  format: yaml
  label: Uptime.com Status Pages API
  slug: uptime-com-status-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-status-pages-api-openapi.yml
- filename: uptime-com-tags-api-openapi.yml
  format: yaml
  label: Uptime.com Tags API
  slug: uptime-com-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/openapi/uptime-com-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uptime Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uptime.com secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Uptime.com
provider_slug: uptime-com
scheme_count: 1
schemes:
- description: 'API token authentication. Pass the header as `Authorization: Token your_api_token`. Tokens are generated from Settings > API in the Uptime.com app and require a paid account.'
  in: header
  name: tokenAuth
  parameter: Authorization
  sources:
  - openapi/uptime-com-openapi.yml
  type: apiKey
slug: uptime-com-authentication
source_filename: uptime-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uptime-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'API token authentication. Pass the header as `Authorization: Token your_api_token`.\n    Tokens are generated from Settings > API in the Uptime.com app and require a paid account.'\n  sources:\n  - openapi/uptime-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uptime-com/refs/heads/main/authentication/uptime-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Monitoring
- Uptime
- Website Monitoring
- Status Pages
- SLA
---
