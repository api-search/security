---
api_key_in:
- cookie
api_specs:
- filename: heyform-auth-api-openapi.yml
  format: yaml
  label: HeyForm Auth API
  slug: heyform-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-auth-api-openapi.yml
- filename: heyform-config-api-openapi.yml
  format: yaml
  label: HeyForm Config API
  slug: heyform-config-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-config-api-openapi.yml
- filename: heyform-forms-api-openapi.yml
  format: yaml
  label: HeyForm Forms API
  slug: heyform-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-forms-api-openapi.yml
- filename: heyform-graphql-api-openapi.yml
  format: yaml
  label: HeyForm GraphQL API
  slug: heyform-graphql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-graphql-api-openapi.yml
- filename: heyform-images-api-openapi.yml
  format: yaml
  label: HeyForm Images API
  slug: heyform-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-images-api-openapi.yml
- filename: heyform-submissions-api-openapi.yml
  format: yaml
  label: HeyForm Submissions API
  slug: heyform-submissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-submissions-api-openapi.yml
- filename: heyform-upload-api-openapi.yml
  format: yaml
  label: HeyForm Upload API
  slug: heyform-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/heyform/refs/heads/main/openapi/heyform-upload-api-openapi.yml
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
- Open-Source
- Webhook
- No-Code
- Form Builder
- Self-Hosted
---
