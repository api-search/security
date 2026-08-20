---
api_key_in: []
api_specs:
- filename: courier-asyncapi.yml
  format: yaml
  label: Courier Inbox Real-Time API
  slug: courier-inbox-real-time-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/asyncapi/courier-asyncapi.yml
- filename: courier-audiences-api-openapi.yml
  format: yaml
  label: Courier Audiences API
  slug: courier-audiences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-audiences-api-openapi.yml
- filename: courier-audit-events-api-openapi.yml
  format: yaml
  label: Courier Audit Events API
  slug: courier-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-audit-events-api-openapi.yml
- filename: courier-authentication-api-openapi.yml
  format: yaml
  label: Courier Authentication API
  slug: courier-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-authentication-api-openapi.yml
- filename: courier-automations-api-openapi.yml
  format: yaml
  label: Courier Automations API
  slug: courier-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-automations-api-openapi.yml
- filename: courier-brands-api-openapi.yml
  format: yaml
  label: Courier Brands API
  slug: courier-brands-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-brands-api-openapi.yml
- filename: courier-bulk-api-openapi.yml
  format: yaml
  label: Courier Bulk API
  slug: courier-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-bulk-api-openapi.yml
- filename: courier-courier-create-api-openapi.yml
  format: yaml
  label: Courier Courier Create API
  slug: courier-courier-create-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-courier-create-api-openapi.yml
- filename: courier-device-tokens-api-openapi.yml
  format: yaml
  label: Courier Device Tokens API
  slug: courier-device-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-device-tokens-api-openapi.yml
- filename: courier-inbound-api-openapi.yml
  format: yaml
  label: Courier Inbound API
  slug: courier-inbound-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-inbound-api-openapi.yml
- filename: courier-journeys-api-openapi.yml
  format: yaml
  label: Courier Journeys API
  slug: courier-journeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-journeys-api-openapi.yml
- filename: courier-lists-api-openapi.yml
  format: yaml
  label: Courier Lists API
  slug: courier-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-lists-api-openapi.yml
- filename: courier-notification-templates-api-openapi.yml
  format: yaml
  label: Courier Notification Templates API
  slug: courier-notification-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-notification-templates-api-openapi.yml
- filename: courier-providers-api-openapi.yml
  format: yaml
  label: Courier Providers API
  slug: courier-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-providers-api-openapi.yml
- filename: courier-routing-strategies-api-openapi.yml
  format: yaml
  label: Courier Routing Strategies API
  slug: courier-routing-strategies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-routing-strategies-api-openapi.yml
- filename: courier-send-api-openapi.yml
  format: yaml
  label: Courier Send API
  slug: courier-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-send-api-openapi.yml
- filename: courier-sent-messages-api-openapi.yml
  format: yaml
  label: Courier Sent Messages API
  slug: courier-sent-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-sent-messages-api-openapi.yml
- filename: courier-tenants-api-openapi.yml
  format: yaml
  label: Courier Tenants API
  slug: courier-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-tenants-api-openapi.yml
- filename: courier-translations-api-openapi.yml
  format: yaml
  label: Courier Translations API
  slug: courier-translations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-translations-api-openapi.yml
- filename: courier-user-preferences-api-openapi.yml
  format: yaml
  label: Courier User Preferences API
  slug: courier-user-preferences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-user-preferences-api-openapi.yml
- filename: courier-user-profiles-api-openapi.yml
  format: yaml
  label: Courier User Profiles API
  slug: courier-user-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-user-profiles-api-openapi.yml
- filename: courier-user-tenants-api-openapi.yml
  format: yaml
  label: Courier User Tenants API
  slug: courier-user-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/openapi/courier-user-tenants-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Courier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Courier secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Courier
provider_slug: courier
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/courier-openapi.yml
  type: http
slug: courier-authentication
source_filename: courier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/courier-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/courier-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/courier/refs/heads/main/authentication/courier-authentication.yml
summary_line: http · 1 scheme
tags:
- Notification
- Email
- SMS
- Push
---
