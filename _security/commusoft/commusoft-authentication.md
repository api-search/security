---
api_key_in:
- header
- query
api_specs:
- filename: commusoft-authentication-api-openapi.yml
  format: yaml
  label: Commusoft Authentication API
  slug: commusoft-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/openapi/commusoft-authentication-api-openapi.yml
- filename: commusoft-contacts-api-openapi.yml
  format: yaml
  label: Commusoft Contacts API
  slug: commusoft-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/openapi/commusoft-contacts-api-openapi.yml
- filename: commusoft-customers-api-openapi.yml
  format: yaml
  label: Commusoft Customers API
  slug: commusoft-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/openapi/commusoft-customers-api-openapi.yml
- filename: commusoft-diary-events-api-openapi.yml
  format: yaml
  label: Commusoft Diary Events API
  slug: commusoft-diary-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/openapi/commusoft-diary-events-api-openapi.yml
- filename: commusoft-locations-api-openapi.yml
  format: yaml
  label: Commusoft Locations API
  slug: commusoft-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/openapi/commusoft-locations-api-openapi.yml
- filename: commusoft-suppliers-api-openapi.yml
  format: yaml
  label: Commusoft Suppliers API
  slug: commusoft-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/openapi/commusoft-suppliers-api-openapi.yml
- filename: commusoft-titles-api-openapi.yml
  format: yaml
  label: Commusoft Titles API
  slug: commusoft-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/openapi/commusoft-titles-api-openapi.yml
- filename: commusoft-users-api-openapi.yml
  format: yaml
  label: Commusoft Users API
  slug: commusoft-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/openapi/commusoft-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Commusoft Authentication
name_suffix: Authentication
oauth_flows: []
overview: Commusoft secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Commusoft
provider_slug: commusoft
scheme_count: 2
schemes:
- description: API token obtained from the /getToken endpoint
  in: header
  name: ApiTokenHeader
  parameter: X-Auth-Token
  sources:
  - openapi/commusoft-api-openapi.yml
  type: apiKey
- description: API token passed as a query parameter
  in: query
  name: ApiTokenQuery
  parameter: token
  sources:
  - openapi/commusoft-api-openapi.yml
  type: apiKey
slug: commusoft-authentication
source_filename: commusoft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/commusoft-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiTokenHeader\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: API token obtained from the /getToken endpoint\n  sources:\n  - openapi/commusoft-api-openapi.yml\n- name: ApiTokenQuery\n  type: apiKey\n  in: query\n  parameter: token\n  description: API token passed as a query parameter\n  sources:\n  - openapi/commusoft-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commusoft/refs/heads/main/authentication/commusoft-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Field Service Management
- Job Management
- HVAC
- Plumbing
- Trades
- Scheduling
- Invoicing
- Engineers
- Customers
- Service History
---
