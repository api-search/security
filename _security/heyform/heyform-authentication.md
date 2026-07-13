---
api_key_in:
- cookie
api_specs:
- filename: heyform-heyform-api-openapi.yml
  format: yaml
  label: HeyForm API
  slug: heyform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-heyform-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Heyform Authentication
name_suffix: Authentication
oauth_flows: []
overview: HeyForm secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HeyForm
provider_slug: heyform
scheme_count: 1
schemes:
- description: Session cookie set by the login mutation or OAuth callback. All authenticated GraphQL mutations and the CSV export endpoint require this cookie.
  in: cookie
  name: cookieAuth
  parameter: heyform_sid
  sources:
  - openapi/heyform-heyform-api-openapi.yml
  type: apiKey
slug: heyform-authentication
source_filename: heyform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/heyform-heyform-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: heyform_sid\n  description: Session cookie set by the login mutation or OAuth callback. All authenticated\n    GraphQL mutations and the CSV export endpoint require this cookie.\n  sources:\n  - openapi/heyform-heyform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/authentication/heyform-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Forms
- Surveys
- Quizzes
- Polls
- Conversational Forms
- Open Source
- Webhooks
- No-Code
- Form Builder
- Self-Hosted
---
