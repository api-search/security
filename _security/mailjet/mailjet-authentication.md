---
api_key_in: []
api_specs:
- filename: mailjet-email-api-openapi.yml
  format: yaml
  label: Mailjet Email API
  slug: mailjet-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-email-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mailjet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailjet secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mailjet
provider_slug: mailjet
scheme_count: 1
schemes:
- description: API key and secret used as HTTP Basic credentials
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/mailjet-email-api-openapi.yml
  type: http
slug: mailjet-authentication
source_filename: mailjet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mailjet-email-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: API key and secret used as HTTP Basic credentials\n  sources:\n  - openapi/mailjet-email-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/authentication/mailjet-authentication.yml
summary_line: http · 1 scheme
tags:
- Email
- Email Delivery
- Marketing Email
- SMTP
- Transactional Email
---
