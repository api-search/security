---
api_key_in: []
api_specs:
- filename: wufoo-webhooks-asyncapi.yml
  format: yaml
  label: Wufoo Webhooks
  slug: wufoo-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/asyncapi/wufoo-webhooks-asyncapi.yml
- filename: wufoo-comments-api-openapi.yml
  format: yaml
  label: Wufoo Comments API
  slug: wufoo-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-comments-api-openapi.yml
- filename: wufoo-entries-api-openapi.yml
  format: yaml
  label: Wufoo Entries API
  slug: wufoo-entries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-entries-api-openapi.yml
- filename: wufoo-fields-api-openapi.yml
  format: yaml
  label: Wufoo Fields API
  slug: wufoo-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-fields-api-openapi.yml
- filename: wufoo-forms-api-openapi.yml
  format: yaml
  label: Wufoo Forms API
  slug: wufoo-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-forms-api-openapi.yml
- filename: wufoo-login-api-openapi.yml
  format: yaml
  label: Wufoo Login API
  slug: wufoo-login-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-login-api-openapi.yml
- filename: wufoo-reports-api-openapi.yml
  format: yaml
  label: Wufoo Reports API
  slug: wufoo-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-reports-api-openapi.yml
- filename: wufoo-users-api-openapi.yml
  format: yaml
  label: Wufoo Users API
  slug: wufoo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-users-api-openapi.yml
- filename: wufoo-webhooks-api-openapi.yml
  format: yaml
  label: Wufoo Webhooks API
  slug: wufoo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-webhooks-api-openapi.yml
- filename: wufoo-widgets-api-openapi.yml
  format: yaml
  label: Wufoo Widgets API
  slug: wufoo-widgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/openapi/wufoo-widgets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Wufoo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wufoo secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wufoo
provider_slug: wufoo
scheme_count: 1
schemes:
- description: 'HTTP Basic Auth. Use your Wufoo API key as the username and any non-empty

    string as the password. Servers require TLS v1.0 or higher; SSLv3 and lower

    are blocked.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/wufoo-rest-v3-openapi.yml
  type: http
slug: wufoo-authentication
source_filename: wufoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wufoo-rest-v3-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic Auth. Use your Wufoo API key as the username and any non-empty\n    string as the password. Servers require TLS v1.0 or higher; SSLv3 and lower\n    are blocked.\n  sources:\n  - openapi/wufoo-rest-v3-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wufoo/refs/heads/main/authentication/wufoo-authentication.yml
summary_line: http · 1 scheme
tags:
- Forms
- Form Builder
- Surveys
- Data Collection
- Webhooks
- Payments
- SurveyMonkey
---
