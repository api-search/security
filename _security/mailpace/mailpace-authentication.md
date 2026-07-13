---
api_key_in:
- header
api_specs:
- filename: mailpace-openapi.yml
  format: yaml
  label: MailPace Send Email API
  slug: mailpace-send-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailpace/refs/heads/main/openapi/mailpace-openapi.yml
- filename: mailpace-openapi.yml
  format: yaml
  label: MailPace Domains API
  slug: mailpace-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailpace/refs/heads/main/openapi/mailpace-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mailpace Authentication
name_suffix: Authentication
oauth_flows: []
overview: MailPace secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: MailPace
provider_slug: mailpace
scheme_count: 2
schemes:
- description: Per-domain server token used to authenticate send requests.
  in: header
  name: ServerToken
  parameter: MailPace-Server-Token
  sources:
  - openapi/mailpace-openapi.yml
  type: apiKey
- description: Organization token used to authenticate domain and token management.
  in: header
  name: OrganizationToken
  parameter: MailPace-Organization-Token
  sources:
  - openapi/mailpace-openapi.yml
  type: apiKey
slug: mailpace-authentication
source_filename: mailpace-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mailpace-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ServerToken\n  type: apiKey\n  in: header\n  parameter: MailPace-Server-Token\n  description: Per-domain server token used to authenticate send requests.\n  sources:\n  - openapi/mailpace-openapi.yml\n- name: OrganizationToken\n  type: apiKey\n  in: header\n  parameter: MailPace-Organization-Token\n  description: Organization token used to authenticate domain and token management.\n  sources:\n  - openapi/mailpace-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailpace/refs/heads/main/authentication/mailpace-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Email
- Transactional Email
- Messaging
- SMTP
- Privacy
---
