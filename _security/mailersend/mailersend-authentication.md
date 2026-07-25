---
api_key_in: []
api_specs:
- filename: mailersend-bulk-email-api-openapi.yml
  format: yaml
  label: MailerSend Bulk Email API
  slug: mailersend-bulk-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-bulk-email-api-openapi.yml
- filename: mailersend-domains-api-openapi.yml
  format: yaml
  label: MailerSend Domains API
  slug: mailersend-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-domains-api-openapi.yml
- filename: mailersend-email-api-openapi.yml
  format: yaml
  label: MailerSend Email API
  slug: mailersend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-email-api-openapi.yml
- filename: mailersend-messages-api-openapi.yml
  format: yaml
  label: MailerSend Messages API
  slug: mailersend-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-messages-api-openapi.yml
- filename: mailersend-sender-identities-api-openapi.yml
  format: yaml
  label: MailerSend Sender Identities API
  slug: mailersend-sender-identities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-sender-identities-api-openapi.yml
- filename: mailersend-templates-api-openapi.yml
  format: yaml
  label: MailerSend Templates API
  slug: mailersend-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-templates-api-openapi.yml
- filename: mailersend-webhooks-api-openapi.yml
  format: yaml
  label: MailerSend Webhooks API
  slug: mailersend-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailersend/refs/heads/main/openapi/mailersend-webhooks-api-openapi.yml
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
