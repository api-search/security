---
api_key_in:
- header
api_specs:
- filename: smtp2go-email-api-openapi.yml
  format: yaml
  label: SMTP2GO Email API
  slug: smtp2go-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/openapi/smtp2go-email-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Smtp2Go Authentication
name_suffix: Authentication
oauth_flows: []
overview: SMTP2GO secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SMTP2GO
provider_slug: smtp2go
scheme_count: 2
schemes:
- description: API key passed as an HTTP header
  in: header
  name: ApiKeyHeader
  parameter: X-Smtp2go-Api-Key
  sources:
  - openapi/smtp2go-email-api-openapi.yml
  type: apiKey
- description: API key can also be included in the JSON request body as the "api_key" field
  in: header
  name: ApiKeyBody
  parameter: api_key
  sources:
  - openapi/smtp2go-email-api-openapi.yml
  type: apiKey
slug: smtp2go-authentication
source_filename: smtp2go-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/smtp2go-email-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Smtp2go-Api-Key\n  description: API key passed as an HTTP header\n  sources:\n  - openapi/smtp2go-email-api-openapi.yml\n- name: ApiKeyBody\n  type: apiKey\n  in: header\n  parameter: api_key\n  description: API key can also be included in the JSON request body as the \"api_key\" field\n  sources:\n  - openapi/smtp2go-email-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smtp2go/refs/heads/main/authentication/smtp2go-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Email
- Email Delivery
- Transactional Email
- SMTP
- SMS
- Email API
- Deliverability
---
