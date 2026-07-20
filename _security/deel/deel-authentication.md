---
api_key_in: []
api_specs:
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel People API
  slug: deel-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Organizations API
  slug: deel-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Contracts API
  slug: deel-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Time Off API
  slug: deel-time-off-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Time Tracking API
  slug: deel-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Payroll API
  slug: deel-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Invoices API
  slug: deel-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Expenses API
  slug: deel-expenses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel EOR API
  slug: deel-eor-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Background Checks API
  slug: deel-background-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Immigration API
  slug: deel-immigration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel IT API
  slug: deel-it-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel SCIM API
  slug: deel-scim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel ATS API
  slug: deel-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Accounting API
  slug: deel-accounting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Lookups API
  slug: deel-lookups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel Webhooks API
  slug: deel-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel OAuth & Apps API
  slug: deel-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
- filename: deel-platform-endpoints-openapi.json
  format: json
  label: Deel MCP Server
  slug: deel-mcp-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/openapi/deel-platform-endpoints-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Deel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Deel secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Deel
provider_slug: deel
scheme_count: 1
schemes:
- description: "## Authentication\nThe Deel API uses bearer tokens to authenticate requests. All API calls must be made over HTTPS — calls over plain HTTP or without authentication will fail.\n\n```curl\ncurl -X GET 'https://api.letsdeel.com/rest/v2/contracts' \\\n  -H 'Authorization: Bearer [example key]'\n```\n\n[Learn more about authentication](/api/authentication)"
  name: deelToken
  scheme: bearer
  sources:
  - openapi/deel-contracts-endpoints-openapi.json
  - openapi/deel-custom-fields-endpoints-openapi.json
  - openapi/deel-endpoints-1-openapi.json
  - openapi/deel-eor-endpoints-openapi.json
  - openapi/deel-eor-worker-endpoints-openapi.json
  - openapi/deel-global-payroll-endpoints-openapi.json
  - openapi/deel-it-endpoints-openapi.json
  - openapi/deel-platform-endpoints-openapi.json
  type: http
slug: deel-authentication
source_filename: deel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/deel-contracts-endpoints-openapi.json, openapi/deel-custom-fields-endpoints-openapi.json,\n  openapi/deel-endpoints-1-openapi.json, openapi/deel-eor-endpoints-openapi.json, openapi/deel-eor-worker-endpoints-openapi.json,\n  openapi/deel-global-payroll-endpoints-openapi.json, openapi/deel-it-endpoints-openapi.json,\n  openapi/deel-platform-endpoints-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: deelToken\n  type: http\n  scheme: bearer\n  description: |-\n    ## Authentication\n    The Deel API uses bearer tokens to authenticate requests. All API calls must be made over HTTPS — calls over plain HTTP or without authentication will fail.\n\n    ```curl\n    curl -X GET 'https://api.letsdeel.com/rest/v2/contracts' \\\n      -H 'Authorization: Bearer [example key]'\n    ```\n\n    [Learn more about authentication](/api/authentication)\n  sources:\n  - openapi/deel-contracts-endpoints-openapi.json\n  - openapi/deel-custom-fields-endpoints-openapi.json\n\
  \  - openapi/deel-endpoints-1-openapi.json\n  - openapi/deel-eor-endpoints-openapi.json\n  - openapi/deel-eor-worker-endpoints-openapi.json\n  - openapi/deel-global-payroll-endpoints-openapi.json\n  - openapi/deel-it-endpoints-openapi.json\n  - openapi/deel-platform-endpoints-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/deel/refs/heads/main/authentication/deel-authentication.yml
summary_line: http · 1 scheme
tags:
- HR
- Payroll
- Global Hiring
- EOR
- Contractors
- Compliance
- SCIM
---
