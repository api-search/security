---
api_key_in: []
api_specs:
- filename: mailgun.yaml
  format: yaml
  label: Mailgun Send API
  slug: send-api
  spec_type: OpenAPI
  url: https://documentation.mailgun.com/_spec/docs/mailgun/api-reference/send/mailgun.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mailgun Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailgun secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mailgun
provider_slug: mailgun
scheme_count: 1
schemes:
- description: HTTP Basic with username `api` and your Mailgun API key as the password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/mailgun-openapi.yml
  type: http
slug: mailgun-authentication
source_filename: mailgun-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mailgun-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with username `api` and your Mailgun API key as the password.\n  sources:\n  - openapi/mailgun-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/authentication/mailgun-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Transactional Email
- SMTP
- Email Validation
- Email Delivery
- Messaging
---
