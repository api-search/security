---
api_key_in: []
api_specs:
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk People API
  slug: folk-app-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Companies API
  slug: folk-app-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Deals and Custom Objects API
  slug: folk-app-deals-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Groups API
  slug: folk-app-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Notes API
  slug: folk-app-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Reminders API
  slug: folk-app-reminders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Interactions API
  slug: folk-app-interactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Users API
  slug: folk-app-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
- filename: folk-app-openapi.yml
  format: yaml
  label: Folk Webhooks API
  slug: folk-app-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/openapi/folk-app-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Folk App Authentication
name_suffix: Authentication
oauth_flows: []
overview: Folk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Folk
provider_slug: folk-app
scheme_count: 1
schemes:
- description: 'API key for authentication, sent as `Authorization: Bearer <api_key>`. Keys are created in workspace settings under "API". API access requires a paid Folk plan.'
  name: bearerApiKeyAuth
  scheme: bearer
  sources:
  - openapi/folk-app-openapi.yml
  type: http
slug: folk-app-authentication
source_filename: folk-app-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/folk-app-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerApiKeyAuth\n  type: http\n  scheme: bearer\n  description: 'API key for authentication, sent as `Authorization: Bearer <api_key>`. Keys\n    are created in workspace settings under \"API\". API access requires a paid Folk plan.'\n  sources:\n  - openapi/folk-app-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/folk-app/refs/heads/main/authentication/folk-app-authentication.yml
summary_line: http · 1 scheme
tags:
- CRM
- Relationships
- Contacts
- Sales
- Pipeline
- Webhooks
---
