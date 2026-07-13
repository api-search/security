---
api_key_in: []
api_specs:
- filename: mailosaur-mailosaur-api-openapi.yml
  format: yaml
  label: Mailosaur API
  slug: mailosaur-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/openapi/mailosaur-mailosaur-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mailosaur Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mailosaur secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mailosaur
provider_slug: mailosaur
scheme_count: 1
schemes:
- description: HTTP Basic Auth using your Mailosaur API key as the username and an empty password, or your API key as both username and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/mailosaur-mailosaur-api-openapi.yml
  type: http
slug: mailosaur-authentication
source_filename: mailosaur-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mailosaur-mailosaur-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Auth using your Mailosaur API key as the username and an empty password,\n    or your API key as both username and password.\n  sources:\n  - openapi/mailosaur-mailosaur-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailosaur/refs/heads/main/authentication/mailosaur-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Testing
- SMS Testing
- Developer Tools
- QA Automation
- CI/CD
- SMTP
- TOTP
- Deliverability
---
