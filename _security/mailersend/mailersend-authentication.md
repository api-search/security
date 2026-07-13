---
api_key_in: []
api_specs:
- filename: mailersend-openapi.yml
  format: yaml
  label: MailerSend API
  slug: mailersend-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mailersend Authentication
name_suffix: Authentication
oauth_flows: []
overview: MailerSend secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MailerSend
provider_slug: mailersend
scheme_count: 1
schemes:
- description: API token generated in MailerSend dashboard.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/mailersend-openapi.yml
  type: http
slug: mailersend-authentication
source_filename: mailersend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mailersend-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API token generated in MailerSend dashboard.\n  sources:\n  - openapi/mailersend-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/authentication/mailersend-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Transactional Email
- SMTP
- Marketing
- Communications
---
