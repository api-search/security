---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailtester-com-agent-gateway-api-openapi.yml
  format: yaml
  label: MailTester Agent Gateway API
  slug: mailtester-com-agent-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtester-com/openapi/mailtester-com-agent-gateway-api-openapi.yml
- filename: mailtester-com-credits-api-openapi.yml
  format: yaml
  label: MailTester Credits API
  slug: mailtester-com-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtester-com/openapi/mailtester-com-credits-api-openapi.yml
- filename: mailtester-com-verify-api-openapi.yml
  format: yaml
  label: MailTester Verify API
  slug: mailtester-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailtester-com/openapi/mailtester-com-verify-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: MailTester Authentication
name_suffix: Authentication
oauth_flows: []
overview: MailTester secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MailTester
provider_slug: mailtester-com
scheme_count: 1
schemes:
- name: bearer
  scheme: bearer
  sources:
  - openapi/mailtester-com-openapi.json
  type: http
slug: mailtester-com-authentication
source_filename: mailtester-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/mailtester-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/mailtester-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/mailtester-com/authentication/mailtester-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Email Verification
- Deliverability Testing
- List Cleaning
- Marketing Tools
---
