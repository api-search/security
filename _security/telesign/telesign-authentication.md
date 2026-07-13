---
api_key_in: []
api_specs:
- filename: telesign-sms-openapi.yml
  format: yaml
  label: Telesign SMS API
  slug: sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-sms-openapi.yml
- filename: telesign-phoneid-openapi.yml
  format: yaml
  label: Telesign PhoneID API
  slug: phoneid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-phoneid-openapi.yml
- filename: telesign-verify-openapi.yml
  format: yaml
  label: Telesign Verify API
  slug: verify-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-verify-openapi.yml
- filename: telesign-score-openapi.yml
  format: yaml
  label: Telesign Score API
  slug: score-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-score-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Telesign Authentication
name_suffix: Authentication
oauth_flows: []
overview: Telesign secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Telesign
provider_slug: telesign
scheme_count: 1
schemes:
- description: Basic authentication using Customer ID as username and API key as password.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/telesign-phoneid-openapi.yml
  - openapi/telesign-score-openapi.yml
  - openapi/telesign-sms-openapi.yml
  - openapi/telesign-verify-openapi.yml
  type: http
slug: telesign-authentication
source_filename: telesign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/telesign-phoneid-openapi.yml, openapi/telesign-score-openapi.yml, openapi/telesign-sms-openapi.yml,\n  openapi/telesign-verify-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication using Customer ID as username and API key as password.\n  sources:\n  - openapi/telesign-phoneid-openapi.yml\n  - openapi/telesign-score-openapi.yml\n  - openapi/telesign-sms-openapi.yml\n  - openapi/telesign-verify-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/authentication/telesign-authentication.yml
summary_line: http · 1 scheme
tags:
- Authentication
- Communications
- Fraud Prevention
- Phone Intelligence
- SMS
- Verification
---
