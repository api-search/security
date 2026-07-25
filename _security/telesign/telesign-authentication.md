---
api_key_in: []
api_specs:
- filename: telesign-fraud-scoring-api-openapi.yml
  format: yaml
  label: Telesign Fraud Scoring API
  slug: telesign-fraud-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-fraud-scoring-api-openapi.yml
- filename: telesign-messaging-api-openapi.yml
  format: yaml
  label: Telesign Messaging API
  slug: telesign-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-messaging-api-openapi.yml
- filename: telesign-phone-intelligence-api-openapi.yml
  format: yaml
  label: Telesign Phone Intelligence API
  slug: telesign-phone-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-phone-intelligence-api-openapi.yml
- filename: telesign-verification-api-openapi.yml
  format: yaml
  label: Telesign Verification API
  slug: telesign-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telesign/refs/heads/main/openapi/telesign-verification-api-openapi.yml
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
