---
api_key_in: []
api_specs:
- filename: wootric-declines-api-openapi.yml
  format: yaml
  label: Wootric Declines API
  slug: wootric-declines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-declines-api-openapi.yml
- filename: wootric-email-surveys-api-openapi.yml
  format: yaml
  label: Wootric Email Surveys API
  slug: wootric-email-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-email-surveys-api-openapi.yml
- filename: wootric-end-users-api-openapi.yml
  format: yaml
  label: Wootric End Users API
  slug: wootric-end-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-end-users-api-openapi.yml
- filename: wootric-metrics-api-openapi.yml
  format: yaml
  label: Wootric Metrics API
  slug: wootric-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-metrics-api-openapi.yml
- filename: wootric-responses-api-openapi.yml
  format: yaml
  label: Wootric Responses API
  slug: wootric-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-responses-api-openapi.yml
- filename: wootric-segments-api-openapi.yml
  format: yaml
  label: Wootric Segments API
  slug: wootric-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-segments-api-openapi.yml
- filename: wootric-settings-api-openapi.yml
  format: yaml
  label: Wootric Settings API
  slug: wootric-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-settings-api-openapi.yml
- filename: wootric-survey-templates-api-openapi.yml
  format: yaml
  label: Wootric Survey Templates API
  slug: wootric-survey-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wootric/refs/heads/main/openapi/wootric-survey-templates-api-openapi.yml
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
- Customer Satisfaction
- Customer Effort Score
- Surveys
- Feedback
- Voice of the Customer
---
