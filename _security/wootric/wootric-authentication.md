---
api_key_in: []
api_specs:
- filename: wootric-openapi.yml
  format: yaml
  label: Wootric API
  slug: wootric-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wootric Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wootric secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wootric
provider_slug: wootric
scheme_count: 1
schemes:
- description: OAuth 2.0 Bearer token. Obtain via password, client_credentials, or refresh_token grant. Tokens expire after 2 hours.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/wootric-openapi.yml
  type: http
slug: wootric-authentication
source_filename: wootric-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wootric-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 Bearer token. Obtain via password, client_credentials, or refresh_token\n    grant. Tokens expire after 2 hours.\n  sources:\n  - openapi/wootric-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/authentication/wootric-authentication.yml
summary_line: http · 1 scheme
tags:
- Customer Experience
- NPS
- CSAT
- CES
- Net Promoter Score
- Customer Satisfaction
- Customer Effort Score
- Surveys
- Feedback
- Voice of the Customer
---
