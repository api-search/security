---
api_key_in:
- header
api_specs:
- filename: prolific-openapi-original.yml
  format: yaml
  label: Prolific API
  slug: prolific-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/openapi/prolific-openapi-original.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Prolific Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prolific secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Prolific
provider_slug: prolific
scheme_count: 1
schemes:
- description: 'The Prolific API uses API token to authenticate requests. You can create an API token directly from your settings.


    Your API token does not have an expiry date and carries full permission, so be sure to keep them secure.


    If your token is leaked, delete it and create a new one directly in the app.


    In your requests add `Authorization` header with the value `Token <your token>`.'
  in: header
  name: token
  parameter: Authorization
  sources:
  - openapi/prolific-openapi-original.yml
  type: apiKey
slug: prolific-authentication
source_filename: prolific-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/prolific-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    The Prolific API uses API token to authenticate requests. You can create an API token directly from your settings.\n\n    Your API token does not have an expiry date and carries full permission, so be sure to keep them secure.\n\n    If your token is leaked, delete it and create a new one directly in the app.\n\n    In your requests add `Authorization` header with the value `Token <your token>`.\n  sources:\n  - openapi/prolific-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prolific/refs/heads/main/authentication/prolific-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai/Ml
- Human Data
- Research
- Participant Recruitment
- Surveys
- Human Feedback
- RLHF
- Data Collection
- API
---
