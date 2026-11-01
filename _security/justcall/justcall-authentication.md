---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: justcall-calls-api-openapi.yml
  format: yaml
  label: JustCall Calls API
  slug: justcall-calls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-calls-api-openapi.yml
- filename: justcall-contacts-api-openapi.yml
  format: yaml
  label: JustCall Contacts API
  slug: justcall-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-contacts-api-openapi.yml
- filename: justcall-sms-api-openapi.yml
  format: yaml
  label: JustCall SMS API
  slug: justcall-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-sms-api-openapi.yml
- filename: justcall-ai-voice-agents-api-openapi.yml
  format: yaml
  label: JustCall AI Voice Agents API
  slug: justcall-ai-voice-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-ai-voice-agents-api-openapi.yml
- filename: justcall-appointments-api-openapi.yml
  format: yaml
  label: JustCall Appointments API
  slug: justcall-appointments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-appointments-api-openapi.yml
- filename: justcall-justcall-ai-api-openapi.yml
  format: yaml
  label: JustCall JustCall AI API
  slug: justcall-justcall-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-justcall-ai-api-openapi.yml
- filename: justcall-oauth-api-openapi.yml
  format: yaml
  label: JustCall OAuth API
  slug: justcall-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-oauth-api-openapi.yml
- filename: justcall-phone-numbers-api-openapi.yml
  format: yaml
  label: JustCall Phone Numbers API
  slug: justcall-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-phone-numbers-api-openapi.yml
- filename: justcall-rcs-api-openapi.yml
  format: yaml
  label: JustCall RCS API
  slug: justcall-rcs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-rcs-api-openapi.yml
- filename: justcall-sales-dialer-api-openapi.yml
  format: yaml
  label: JustCall Sales Dialer API
  slug: justcall-sales-dialer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-sales-dialer-api-openapi.yml
- filename: justcall-sales-dialer-phone-numbers-api-openapi.yml
  format: yaml
  label: JustCall Sales Dialer - Phone Numbers API
  slug: justcall-sales-dialer-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-sales-dialer-phone-numbers-api-openapi.yml
- filename: justcall-special-dates-api-openapi.yml
  format: yaml
  label: JustCall Special Dates API
  slug: justcall-special-dates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-special-dates-api-openapi.yml
- filename: justcall-unified-analytics-api-openapi.yml
  format: yaml
  label: JustCall Unified Analytics API
  slug: justcall-unified-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-unified-analytics-api-openapi.yml
- filename: justcall-user-groups-api-openapi.yml
  format: yaml
  label: JustCall User Groups API
  slug: justcall-user-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-user-groups-api-openapi.yml
- filename: justcall-users-api-openapi.yml
  format: yaml
  label: JustCall Users API
  slug: justcall-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-users-api-openapi.yml
- filename: justcall-webhooks-api-openapi.yml
  format: yaml
  label: JustCall Webhooks API
  slug: justcall-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-webhooks-api-openapi.yml
- filename: justcall-whats-app-api-openapi.yml
  format: yaml
  label: JustCall Whats App API
  slug: justcall-whats-app-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/justcall/openapi/justcall-whats-app-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Justcall Authentication
name_suffix: Authentication
oauth_flows: []
overview: JustCall secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JustCall
provider_slug: justcall
scheme_count: 1
schemes:
- description: JustCall authentication. Pass the API key and API secret as defined in the JustCall Authentication documentation (typically combined and passed in the Authorization header).
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/justcall-openapi.yml
  type: apiKey
slug: justcall-authentication
source_filename: justcall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/justcall-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: JustCall authentication. Pass the API key and API secret as defined in the JustCall\n    Authentication documentation (typically combined and passed in the Authorization header).\n  sources:\n  - openapi/justcall-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/justcall/authentication/justcall-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Voice
- SMS
- Cloud Phone
- Contact Center
- Telephony
- Communications
---
