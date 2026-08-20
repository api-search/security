---
api_key_in: []
api_specs:
- filename: folk-companies-api-openapi.yml
  format: yaml
  label: Folk Companies API
  slug: folk-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/openapi/folk-companies-api-openapi.yml
- filename: folk-deals-api-openapi.yml
  format: yaml
  label: Folk Deals API
  slug: folk-deals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/openapi/folk-deals-api-openapi.yml
- filename: folk-groups-api-openapi.yml
  format: yaml
  label: Folk Groups API
  slug: folk-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/openapi/folk-groups-api-openapi.yml
- filename: folk-interactions-api-openapi.yml
  format: yaml
  label: Folk Interactions API
  slug: folk-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/openapi/folk-interactions-api-openapi.yml
- filename: folk-notes-api-openapi.yml
  format: yaml
  label: Folk Notes API
  slug: folk-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/openapi/folk-notes-api-openapi.yml
- filename: folk-people-api-openapi.yml
  format: yaml
  label: Folk People API
  slug: folk-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/openapi/folk-people-api-openapi.yml
- filename: folk-reminders-api-openapi.yml
  format: yaml
  label: Folk Reminders API
  slug: folk-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/openapi/folk-reminders-api-openapi.yml
- filename: folk-users-api-openapi.yml
  format: yaml
  label: Folk Users API
  slug: folk-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/openapi/folk-users-api-openapi.yml
- filename: folk-webhooks-api-openapi.yml
  format: yaml
  label: Folk Webhooks API
  slug: folk-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/openapi/folk-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Folk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Folk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Folk
provider_slug: folk
scheme_count: 1
schemes:
- description: API key for authentication
  name: bearerApiKeyAuth
  scheme: bearer
  sources:
  - openapi/folk-openapi.yml
  type: http
slug: folk-authentication
source_filename: folk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/folk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerApiKeyAuth\n  type: http\n  scheme: bearer\n  description: API key for authentication\n  sources:\n  - openapi/folk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/folk/refs/heads/main/authentication/folk-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Contacts
- Pipelines
- Sales
- Relationships
- Notes
- Deals
- Webhook
---
