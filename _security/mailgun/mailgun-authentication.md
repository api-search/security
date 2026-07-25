---
api_key_in: []
api_specs:
- filename: mailgun-domains-api-openapi.yml
  format: yaml
  label: Mailgun Domains API
  slug: mailgun-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-domains-api-openapi.yml
- filename: mailgun-events-api-openapi.yml
  format: yaml
  label: Mailgun Events API
  slug: mailgun-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-events-api-openapi.yml
- filename: mailgun-mailing-lists-api-openapi.yml
  format: yaml
  label: Mailgun Mailing Lists API
  slug: mailgun-mailing-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-mailing-lists-api-openapi.yml
- filename: mailgun-messages-api-openapi.yml
  format: yaml
  label: Mailgun Messages API
  slug: mailgun-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-messages-api-openapi.yml
- filename: mailgun-routes-api-openapi.yml
  format: yaml
  label: Mailgun Routes API
  slug: mailgun-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-routes-api-openapi.yml
- filename: mailgun-suppressions-api-openapi.yml
  format: yaml
  label: Mailgun Suppressions API
  slug: mailgun-suppressions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-suppressions-api-openapi.yml
- filename: mailgun-webhooks-api-openapi.yml
  format: yaml
  label: Mailgun Webhooks API
  slug: mailgun-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/openapi/mailgun-webhooks-api-openapi.yml
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
