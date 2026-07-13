---
api_key_in: []
api_specs:
- filename: mailerlite-openapi.yml
  format: yaml
  label: MailerLite API
  slug: mailerlite-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailerlite/refs/heads/main/openapi/mailerlite-openapi.yml
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
