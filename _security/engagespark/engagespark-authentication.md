---
api_key_in: []
api_specs:
- filename: engagespark-openapi-original.yml
  format: yaml
  label: engageSPARK API
  slug: engagespark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagespark/refs/heads/main/openapi/engagespark-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Engagespark Authentication
name_suffix: Authentication
oauth_flows: []
overview: engageSPARK secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: engageSPARK
provider_slug: engagespark
scheme_count: 1
schemes:
- bearerFormat: token
  description: "Token based HTTP authentication.\n\nUse the header \"Authorization\". The value must be the word \"Token\" followed by your token. For example: \"Authorization: Token aaa111bbb222ccc333\", NOT \"Authorization: aaa111bbb222ccc333\".\n\nAccess tokens can be retrieved and managed [in your User profile](https://app.engagespark.com/profile/api-tokens).\n\nAllowed headers:\n\n  - Authorization: Token [PERSONAL_ACCESS_T"
  name: apiToken
  scheme: token
  sources:
  - openapi/engagespark-openapi-original.yml
  type: http
slug: engagespark-authentication
source_filename: engagespark-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/engagespark-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiToken\n  type: http\n  scheme: token\n  bearerFormat: token\n  description: |-\n    Token based HTTP authentication.\n\n    Use the header \"Authorization\". The value must be the word \"Token\" followed by your token. For example: \"Authorization: Token aaa111bbb222ccc333\", NOT \"Authorization: aaa111bbb222ccc333\".\n\n    Access tokens can be retrieved and managed [in your User profile](https://app.engagespark.com/profile/api-tokens).\n\n    Allowed headers:\n\n      - Authorization: Token [PERSONAL_ACCESS_T\n  sources:\n  - openapi/engagespark-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engagespark/refs/heads/main/authentication/engagespark-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Messaging
- SMS
- Voice
- WhatsApp
- Airtime
- Communications
- CPaaS
- Surveys
- International Development
---
