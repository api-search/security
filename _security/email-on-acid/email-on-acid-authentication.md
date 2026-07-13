---
api_key_in: []
api_specs:
- filename: email-on-acid-openapi.yml
  format: yaml
  label: Email on Acid API
  slug: email-on-acid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/email-on-acid/refs/heads/main/openapi/email-on-acid-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Email On Acid Authentication
name_suffix: Authentication
oauth_flows: []
overview: Email on Acid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Email on Acid
provider_slug: email-on-acid
scheme_count: 1
schemes:
- description: HTTP Basic Authentication using `<api_key>:<account_password>` base64-encoded. Use "sandbox:sandbox" credentials for sandbox testing.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/email-on-acid-openapi.yml
  type: http
slug: email-on-acid-authentication
source_filename: email-on-acid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/email-on-acid-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using `<api_key>:<account_password>` base64-encoded.\n    Use \"sandbox:sandbox\" credentials for sandbox testing.\n  sources:\n  - openapi/email-on-acid-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/email-on-acid/refs/heads/main/authentication/email-on-acid-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Testing
- Email Previews
- Email Clients
- Spam Testing
- Accessibility
- HTML Validation
- Email Quality Assurance
- Pre-Deployment Testing
---
