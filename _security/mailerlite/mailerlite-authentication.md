---
api_key_in: []
api_specs:
- filename: mailerlite-automations-api-openapi.yml
  format: yaml
  label: MailerLite Automations API
  slug: mailerlite-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-automations-api-openapi.yml
- filename: mailerlite-campaigns-api-openapi.yml
  format: yaml
  label: MailerLite Campaigns API
  slug: mailerlite-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-campaigns-api-openapi.yml
- filename: mailerlite-fields-api-openapi.yml
  format: yaml
  label: MailerLite Fields API
  slug: mailerlite-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-fields-api-openapi.yml
- filename: mailerlite-forms-api-openapi.yml
  format: yaml
  label: MailerLite Forms API
  slug: mailerlite-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-forms-api-openapi.yml
- filename: mailerlite-groups-api-openapi.yml
  format: yaml
  label: MailerLite Groups API
  slug: mailerlite-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-groups-api-openapi.yml
- filename: mailerlite-segments-api-openapi.yml
  format: yaml
  label: MailerLite Segments API
  slug: mailerlite-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-segments-api-openapi.yml
- filename: mailerlite-subscribers-api-openapi.yml
  format: yaml
  label: MailerLite Subscribers API
  slug: mailerlite-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-subscribers-api-openapi.yml
- filename: mailerlite-webhooks-api-openapi.yml
  format: yaml
  label: MailerLite Webhooks API
  slug: mailerlite-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mailerlite Authentication
name_suffix: Authentication
oauth_flows: []
overview: MailerLite secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MailerLite
provider_slug: mailerlite
scheme_count: 1
schemes:
- description: Bearer token generated under Integrations > MailerLite API in the dashboard.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/mailerlite-openapi.yml
  type: http
slug: mailerlite-authentication
source_filename: mailerlite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mailerlite-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token generated under Integrations > MailerLite API in the dashboard.\n  sources:\n  - openapi/mailerlite-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/authentication/mailerlite-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Marketing
- Automation
- Newsletters
- Subscribers
---
