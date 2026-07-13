---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Airslate Authentication
name_suffix: Authentication
oauth_flows: []
overview: airSlate secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: airSlate
provider_slug: airslate
scheme_count: 2
schemes:
- description: 'HTTP Basic auth carrying the application Basic Token (base64 of

    client_id:client_secret) used against POST /oauth2/token.'
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/airslate-openapi.yml
  type: http
- description: 'OAuth 2.0 bearer access token issued by /oauth2/token. Required on

    all resource endpoints.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/airslate-openapi.yml
  type: http
slug: airslate-authentication
source_filename: airslate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/airslate-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth carrying the application Basic Token (base64 of\n    client_id:client_secret) used against POST /oauth2/token.\n  sources:\n  - openapi/airslate-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    OAuth 2.0 bearer access token issued by /oauth2/token. Required on\n    all resource endpoints.\n  sources:\n  - openapi/airslate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airslate/refs/heads/main/authentication/airslate-authentication.yml
summary_line: http · 2 schemes
tags:
- Document Automation
- eSignature
- Workflow
- PDF
- No-Code
- AI
---
