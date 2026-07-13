---
api_key_in: []
api_specs:
- filename: authsignal-openapi.yml
  format: yaml
  label: Authsignal Server API
  slug: server-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/openapi/authsignal-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Authsignal Authentication
name_suffix: Authentication
oauth_flows: []
overview: Authsignal secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Authsignal
provider_slug: authsignal
scheme_count: 1
schemes:
- description: 'HTTP Basic auth where the username is the Authsignal tenant secret API

    key and the password is empty.'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/authsignal-openapi.yml
  type: http
slug: authsignal-authentication
source_filename: authsignal-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/authsignal-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: |-\n    HTTP Basic auth where the username is the Authsignal tenant secret API\n    key and the password is empty.\n  sources:\n  - openapi/authsignal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/authsignal/refs/heads/main/authentication/authsignal-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Passkeys
- MFA
- Step-Up
- Passwordless
- Risk
- Biometrics
- Identity Verification
---
