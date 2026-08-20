---
api_key_in: []
api_specs:
- filename: basecamp-webhooks-asyncapi.yml
  format: yaml
  label: Basecamp Webhooks
  slug: basecamp-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/asyncapi/basecamp-webhooks-asyncapi.yml
- filename: basecamp-authorization-api-openapi.yml
  format: yaml
  label: Basecamp Authorization API
  slug: basecamp-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-authorization-api-openapi.yml
- filename: basecamp-campfires-api-openapi.yml
  format: yaml
  label: Basecamp Campfires API
  slug: basecamp-campfires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-campfires-api-openapi.yml
- filename: basecamp-card-tables-api-openapi.yml
  format: yaml
  label: Basecamp Card Tables API
  slug: basecamp-card-tables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-card-tables-api-openapi.yml
- filename: basecamp-comments-api-openapi.yml
  format: yaml
  label: Basecamp Comments API
  slug: basecamp-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-comments-api-openapi.yml
- filename: basecamp-documents-api-openapi.yml
  format: yaml
  label: Basecamp Documents API
  slug: basecamp-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-documents-api-openapi.yml
- filename: basecamp-identity-api-openapi.yml
  format: yaml
  label: Basecamp Identity API
  slug: basecamp-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-identity-api-openapi.yml
- filename: basecamp-messages-api-openapi.yml
  format: yaml
  label: Basecamp Messages API
  slug: basecamp-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-messages-api-openapi.yml
- filename: basecamp-people-api-openapi.yml
  format: yaml
  label: Basecamp People API
  slug: basecamp-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-people-api-openapi.yml
- filename: basecamp-projects-api-openapi.yml
  format: yaml
  label: Basecamp Projects API
  slug: basecamp-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-projects-api-openapi.yml
- filename: basecamp-recordings-api-openapi.yml
  format: yaml
  label: Basecamp Recordings API
  slug: basecamp-recordings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-recordings-api-openapi.yml
- filename: basecamp-schedule-entries-api-openapi.yml
  format: yaml
  label: Basecamp Schedule Entries API
  slug: basecamp-schedule-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-schedule-entries-api-openapi.yml
- filename: basecamp-schedules-api-openapi.yml
  format: yaml
  label: Basecamp Schedules API
  slug: basecamp-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-schedules-api-openapi.yml
- filename: basecamp-subscriptions-api-openapi.yml
  format: yaml
  label: Basecamp Subscriptions API
  slug: basecamp-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-subscriptions-api-openapi.yml
- filename: basecamp-templates-api-openapi.yml
  format: yaml
  label: Basecamp Templates API
  slug: basecamp-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-templates-api-openapi.yml
- filename: basecamp-to-do-lists-api-openapi.yml
  format: yaml
  label: Basecamp To-Do Lists API
  slug: basecamp-to-do-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-to-do-lists-api-openapi.yml
- filename: basecamp-to-dos-api-openapi.yml
  format: yaml
  label: Basecamp To-Dos API
  slug: basecamp-to-dos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-to-dos-api-openapi.yml
- filename: basecamp-token-api-openapi.yml
  format: yaml
  label: Basecamp Token API
  slug: basecamp-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-token-api-openapi.yml
- filename: basecamp-uploads-api-openapi.yml
  format: yaml
  label: Basecamp Uploads API
  slug: basecamp-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-uploads-api-openapi.yml
- filename: basecamp-webhooks-api-openapi.yml
  format: yaml
  label: Basecamp Webhooks API
  slug: basecamp-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/openapi/basecamp-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Basecamp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Basecamp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Basecamp
provider_slug: basecamp
scheme_count: 1
schemes:
- description: 'OAuth 2.0 Bearer token obtained via the Basecamp authorization code flow at launchpad.37signals.com. Include as "Authorization: Bearer {token}" in all requests.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/basecamp-api-openapi.yml
  - openapi/basecamp-oauth-openapi.yml
  type: http
slug: basecamp-authentication
source_filename: basecamp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/basecamp-api-openapi.yml, openapi/basecamp-oauth-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth 2.0 Bearer token obtained via the Basecamp authorization code flow at\n    launchpad.37signals.com. Include as \"Authorization: Bearer {token}\" in all requests.'\n  sources:\n  - openapi/basecamp-api-openapi.yml\n  - openapi/basecamp-oauth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/basecamp/refs/heads/main/authentication/basecamp-authentication.yml
summary_line: http · 1 scheme
tags:
- Collaboration
- Project Management
- REST
- Software-as-a-Service
- Team Communication
---
