---
api_key_in: []
api_specs:
- filename: twenty-crm-companies-api-openapi.yml
  format: yaml
  label: Twenty Companies API
  slug: twenty-crm-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-companies-api-openapi.yml
- filename: twenty-crm-metadata-fields-api-openapi.yml
  format: yaml
  label: Twenty Metadata - Fields API
  slug: twenty-crm-metadata-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-metadata-fields-api-openapi.yml
- filename: twenty-crm-metadata-objects-api-openapi.yml
  format: yaml
  label: Twenty Metadata - Objects API
  slug: twenty-crm-metadata-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-metadata-objects-api-openapi.yml
- filename: twenty-crm-notes-api-openapi.yml
  format: yaml
  label: Twenty Notes API
  slug: twenty-crm-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-notes-api-openapi.yml
- filename: twenty-crm-opportunities-api-openapi.yml
  format: yaml
  label: Twenty Opportunities API
  slug: twenty-crm-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-opportunities-api-openapi.yml
- filename: twenty-crm-people-api-openapi.yml
  format: yaml
  label: Twenty People API
  slug: twenty-crm-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-people-api-openapi.yml
- filename: twenty-crm-tasks-api-openapi.yml
  format: yaml
  label: Twenty Tasks API
  slug: twenty-crm-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/openapi/twenty-crm-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Twenty Crm Authentication
name_suffix: Authentication
oauth_flows: []
overview: Twenty secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Twenty
provider_slug: twenty-crm
scheme_count: 1
schemes:
- bearerFormat: API Key
  description: 'API key created in Settings -> API & Webhooks, sent as `Authorization: Bearer <API_KEY>`.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/twenty-crm-openapi.yml
  type: http
slug: twenty-crm-authentication
source_filename: twenty-crm-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/twenty-crm-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Key\n  description: 'API key created in Settings -> API & Webhooks, sent as `Authorization: Bearer\n    <API_KEY>`.'\n  sources:\n  - openapi/twenty-crm-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/twenty-crm/refs/heads/main/authentication/twenty-crm-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Open Source
- Sales
- GraphQL
- REST
---
