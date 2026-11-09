---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dailylogdesk-com-dataset-api-openapi.yml
  format: yaml
  label: DailyLogDesk Dataset API
  slug: dailylogdesk-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dailylogdesk-com/openapi/dailylogdesk-com-dataset-api-openapi.yml
- filename: dailylogdesk-com-mcp-api-openapi.yml
  format: yaml
  label: DailyLogDesk MCP API
  slug: dailylogdesk-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dailylogdesk-com/openapi/dailylogdesk-com-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Dailylogdesk Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DailyLogDesk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DailyLogDesk
provider_slug: dailylogdesk-com
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/dailylogdesk-com-openapi.yml
  type: http
slug: dailylogdesk-com-authentication
source_filename: dailylogdesk-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/dailylogdesk-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/dailylogdesk-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/dailylogdesk-com/authentication/dailylogdesk-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Construction
- Site Records
- Incident Reporting
- Risk Assessment
- Health and Safety
- Contractors
- Quotes
---
