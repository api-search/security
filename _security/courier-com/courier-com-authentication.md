---
api_key_in: []
api_specs:
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Send API
  slug: courier-com-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Messages API
  slug: courier-com-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Lists API
  slug: courier-com-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier User Profiles API
  slug: courier-com-user-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier User Preferences API
  slug: courier-com-user-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Device Tokens API
  slug: courier-com-device-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Notification Templates API
  slug: courier-com-notification-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Brands API
  slug: courier-com-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Automations API
  slug: courier-com-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Audiences API
  slug: courier-com-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Tenants API
  slug: courier-com-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Bulk API
  slug: courier-com-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Audit Events API
  slug: courier-com-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
- filename: courier-com-openapi.yml
  format: yaml
  label: Courier Translations API
  slug: courier-com-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/openapi/courier-com-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Courier Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Courier secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Courier
provider_slug: courier-com
scheme_count: 1
schemes:
- description: 'Courier API key passed as `Authorization: Bearer <YOUR_API_KEY>`. Keys are found in the Courier settings under API Keys and are environment scoped (test vs production).'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/courier-com-openapi.yml
  type: http
slug: courier-com-authentication
source_filename: courier-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/courier-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Courier API key passed as `Authorization: Bearer <YOUR_API_KEY>`. Keys are found\n    in the Courier settings under API Keys and are environment scoped (test vs production).'\n  sources:\n  - openapi/courier-com-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/courier-com/refs/heads/main/authentication/courier-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Notifications
- Messaging
- Email
- SMS
- Push
- Multi-Channel
- Notification Infrastructure
- In-App Inbox
---
