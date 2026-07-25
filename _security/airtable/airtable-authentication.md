---
api_key_in: []
api_specs:
- filename: airtable-enterprise-api-openapi.yml
  format: yaml
  label: Airtable Enterprise API
  slug: airtable-enterprise-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-enterprise-api-openapi.yml
- filename: airtable-audit-logs-api-openapi.yml
  format: yaml
  label: Airtable Audit Logs API
  slug: airtable-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-audit-logs-api-openapi.yml
- filename: airtable-shares-api-openapi.yml
  format: yaml
  label: Airtable Shares API
  slug: airtable-shares-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-shares-api-openapi.yml
- filename: airtable-bases-api-openapi.yml
  format: yaml
  label: Airtable Bases API
  slug: airtable-bases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-bases-api-openapi.yml
- filename: airtable-comments-api-openapi.yml
  format: yaml
  label: Airtable Comments API
  slug: airtable-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-comments-api-openapi.yml
- filename: airtable-fields-api-openapi.yml
  format: yaml
  label: Airtable Fields API
  slug: airtable-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-fields-api-openapi.yml
- filename: airtable-groups-api-openapi.yml
  format: yaml
  label: Airtable Groups API
  slug: airtable-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-groups-api-openapi.yml
- filename: airtable-records-api-openapi.yml
  format: yaml
  label: Airtable Records API
  slug: airtable-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-records-api-openapi.yml
- filename: airtable-tables-api-openapi.yml
  format: yaml
  label: Airtable Tables API
  slug: airtable-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-tables-api-openapi.yml
- filename: airtable-users-api-openapi.yml
  format: yaml
  label: Airtable Users API
  slug: airtable-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-users-api-openapi.yml
- filename: airtable-webhooks-api-openapi.yml
  format: yaml
  label: Airtable Webhooks API
  slug: airtable-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-webhooks-api-openapi.yml
- filename: airtable-workspaces-api-openapi.yml
  format: yaml
  label: Airtable Workspaces API
  slug: airtable-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/openapi/airtable-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Airtable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Airtable secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Airtable
provider_slug: airtable
scheme_count: 1
schemes:
- description: Airtable uses Bearer token authentication. Provide a personal access token or OAuth access token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/airtable-airtable-api-openapi.yml
  - openapi/airtable-audit-logs-api-openapi.yml
  - openapi/airtable-enterprise-api-openapi.yml
  - openapi/airtable-metadata-api-openapi.yml
  - openapi/airtable-scim-api-openapi.yml
  - openapi/airtable-shares-api-openapi.yml
  type: http
slug: airtable-authentication
source_filename: airtable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airtable-airtable-api-openapi.yml, openapi/airtable-audit-logs-api-openapi.yml,\n  openapi/airtable-enterprise-api-openapi.yml, openapi/airtable-metadata-api-openapi.yml, openapi/airtable-scim-api-openapi.yml,\n  openapi/airtable-shares-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Airtable uses Bearer token authentication. Provide a personal access token or\n    OAuth access token in the Authorization header.\n  sources:\n  - openapi/airtable-airtable-api-openapi.yml\n  - openapi/airtable-audit-logs-api-openapi.yml\n  - openapi/airtable-enterprise-api-openapi.yml\n  - openapi/airtable-metadata-api-openapi.yml\n  - openapi/airtable-scim-api-openapi.yml\n  - openapi/airtable-shares-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airtable/refs/heads/main/authentication/airtable-authentication.yml
summary_line: http · 1 scheme
tags:
- Applications
- Collaboration
- Data
- Databases
- Low-Code
- Productivity
- Spreadsheets
---
