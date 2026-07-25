---
api_key_in: []
api_specs:
- filename: mailjet-campaigns-api-openapi.yml
  format: yaml
  label: Mailjet Campaigns API
  slug: mailjet-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-campaigns-api-openapi.yml
- filename: mailjet-contact-lists-api-openapi.yml
  format: yaml
  label: Mailjet Contact Lists API
  slug: mailjet-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-contact-lists-api-openapi.yml
- filename: mailjet-contacts-api-openapi.yml
  format: yaml
  label: Mailjet Contacts API
  slug: mailjet-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-contacts-api-openapi.yml
- filename: mailjet-event-api-openapi.yml
  format: yaml
  label: Mailjet Event API
  slug: mailjet-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-event-api-openapi.yml
- filename: mailjet-send-api-openapi.yml
  format: yaml
  label: Mailjet Send API
  slug: mailjet-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-send-api-openapi.yml
- filename: mailjet-senders-api-openapi.yml
  format: yaml
  label: Mailjet Senders API
  slug: mailjet-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-senders-api-openapi.yml
- filename: mailjet-statistics-api-openapi.yml
  format: yaml
  label: Mailjet Statistics API
  slug: mailjet-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-statistics-api-openapi.yml
- filename: mailjet-templates-api-openapi.yml
  format: yaml
  label: Mailjet Templates API
  slug: mailjet-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-templates-api-openapi.yml
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
