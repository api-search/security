---
api_key_in: []
api_specs:
- filename: grist-attachments-api-openapi.yml
  format: yaml
  label: Grist attachments API
  slug: grist-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-attachments-api-openapi.yml
- filename: grist-columns-api-openapi.yml
  format: yaml
  label: Grist columns API
  slug: grist-columns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-columns-api-openapi.yml
- filename: grist-data-api-openapi.yml
  format: yaml
  label: Grist data API
  slug: grist-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-data-api-openapi.yml
- filename: grist-docs-api-openapi.yml
  format: yaml
  label: Grist docs API
  slug: grist-docs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-docs-api-openapi.yml
- filename: grist-forms-api-openapi.yml
  format: yaml
  label: Grist forms API
  slug: grist-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-forms-api-openapi.yml
- filename: grist-orgs-api-openapi.yml
  format: yaml
  label: Grist orgs API
  slug: grist-orgs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-orgs-api-openapi.yml
- filename: grist-profile-api-openapi.yml
  format: yaml
  label: Grist profile API
  slug: grist-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-profile-api-openapi.yml
- filename: grist-records-api-openapi.yml
  format: yaml
  label: Grist records API
  slug: grist-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-records-api-openapi.yml
- filename: grist-service-accounts-api-openapi.yml
  format: yaml
  label: Grist service accounts API
  slug: grist-service-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-service-accounts-api-openapi.yml
- filename: grist-session-api-openapi.yml
  format: yaml
  label: Grist session API
  slug: grist-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-session-api-openapi.yml
- filename: grist-sql-api-openapi.yml
  format: yaml
  label: Grist sql API
  slug: grist-sql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-sql-api-openapi.yml
- filename: grist-tables-api-openapi.yml
  format: yaml
  label: Grist tables API
  slug: grist-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-tables-api-openapi.yml
- filename: grist-templates-api-openapi.yml
  format: yaml
  label: Grist templates API
  slug: grist-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-templates-api-openapi.yml
- filename: grist-users-api-openapi.yml
  format: yaml
  label: Grist users API
  slug: grist-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-users-api-openapi.yml
- filename: grist-webhooks-api-openapi.yml
  format: yaml
  label: Grist webhooks API
  slug: grist-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-webhooks-api-openapi.yml
- filename: grist-widgets-api-openapi.yml
  format: yaml
  label: Grist widgets API
  slug: grist-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-widgets-api-openapi.yml
- filename: grist-workspaces-api-openapi.yml
  format: yaml
  label: Grist workspaces API
  slug: grist-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/openapi/grist-workspaces-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Grist Authentication
name_suffix: Authentication
oauth_flows: []
overview: Grist secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Grist
provider_slug: grist
scheme_count: 1
schemes:
- bearerFormat: 'Authorization: Bearer [example key]'
  description: Access to the Grist API is controlled by an Authorization header, which should contain the word 'Bearer', followed by a space, followed by your API key.
  name: ApiKey
  scheme: bearer
  sources:
  - openapi/grist-rest-api-openapi.yml
  type: http
slug: grist-authentication
source_filename: grist-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/grist-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKey\n  type: http\n  scheme: bearer\n  bearerFormat: 'Authorization: Bearer [example key]'\n  description: Access to the Grist API is controlled by an Authorization header, which should\n    contain the word 'Bearer', followed by a space, followed by your API key.\n  sources:\n  - openapi/grist-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/grist/refs/heads/main/authentication/grist-authentication.yml
summary_line: http · 1 scheme
tags:
- Spreadsheet
- Database
- Collaboration
- No-Code
- Data Management
- Webhook
- Open-Source
---
