---
api_key_in: []
api_specs:
- filename: wufoo-rest-v3-openapi.yml
  format: yaml
  label: Wufoo REST API v3
  slug: wufoo:rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo:wufoo/refs/heads/main/openapi/wufoo-rest-v3-openapi.yml
- filename: wufoo-webhooks-asyncapi.yml
  format: yaml
  label: Wufoo Webhooks
  slug: wufoo:webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wufoo:wufoo/refs/heads/main/asyncapi/wufoo-webhooks-asyncapi.yml
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
provider_slug: wufoo:wufoo
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wufoo:wufoo/refs/heads/main/authentication/wufoo-authentication.yml
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
