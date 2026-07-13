---
api_key_in:
- query
api_specs:
- filename: mailboxlayer-openapi.yml
  format: yaml
  label: mailboxlayer Verification API
  slug: mailboxlayer-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailboxlayer/refs/heads/main/openapi/mailboxlayer-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mailboxlayer Authentication
name_suffix: Authentication
oauth_flows: []
overview: mailboxlayer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: mailboxlayer
provider_slug: mailboxlayer
scheme_count: 1
schemes:
- description: API access key provided when you sign up for a mailboxlayer plan.
  in: query
  name: AccessKeyAuth
  parameter: access_key
  sources:
  - openapi/mailboxlayer-openapi.yml
  type: apiKey
slug: mailboxlayer-authentication
source_filename: mailboxlayer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mailboxlayer-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: AccessKeyAuth\n  type: apiKey\n  in: query\n  parameter: access_key\n  description: API access key provided when you sign up for a mailboxlayer plan.\n  sources:\n  - openapi/mailboxlayer-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailboxlayer/refs/heads/main/authentication/mailboxlayer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Email
- Email Verification
- Email Validation
- SMTP
- MX Records
- Catch-All Detection
- Disposable Email
- Free Email Provider
- Role Address
- Quality Score
- apilayer
- Public APIs
---
