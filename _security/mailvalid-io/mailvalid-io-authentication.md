---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailvalid-io-credits-api-openapi.yml
  format: yaml
  label: MailValid Credits API
  slug: mailvalid-io-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailvalid-io/openapi/mailvalid-io-credits-api-openapi.yml
- filename: mailvalid-io-verification-api-openapi.yml
  format: yaml
  label: MailValid Verification API
  slug: mailvalid-io-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailvalid-io/openapi/mailvalid-io-verification-api-openapi.yml
- filename: mailvalid-io-webhooks-api-openapi.yml
  format: yaml
  label: MailValid Webhooks API
  slug: mailvalid-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailvalid-io/openapi/mailvalid-io-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MailValid Authentication
name_suffix: Authentication
oauth_flows: []
overview: MailValid secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MailValid
provider_slug: mailvalid-io
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/mailvalid-io-openapi.yml
  type: http
slug: mailvalid-io-authentication
source_filename: mailvalid-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/mailvalid-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/mailvalid-io-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/mailvalid-io/authentication/mailvalid-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Verification
- Data Hygiene
- API Service
- Software-as-a-Service
- B2B
---
