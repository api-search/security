---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sendbridge-com-account-api-openapi.yml
  format: yaml
  label: SendBridge Account API
  slug: sendbridge-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-account-api-openapi.yml
- filename: sendbridge-com-dmarc-api-openapi.yml
  format: yaml
  label: SendBridge DMARC API
  slug: sendbridge-com-dmarc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-dmarc-api-openapi.yml
- filename: sendbridge-com-mail-tester-api-openapi.yml
  format: yaml
  label: SendBridge Mail Tester API
  slug: sendbridge-com-mail-tester-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-mail-tester-api-openapi.yml
- filename: sendbridge-com-validation-api-openapi.yml
  format: yaml
  label: SendBridge Validation API
  slug: sendbridge-com-validation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/sendbridge-com/openapi/sendbridge-com-validation-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Sendbridge Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: SendBridge declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: SendBridge
provider_slug: sendbridge-com
scheme_count: 1
schemes:
- description: API key passed as Bearer token. Prefix `sbk_live_` for production or `sbk_test_` for test.
  type: bearer
slug: sendbridge-com-authentication
source_filename: sendbridge-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: derived\nsource: https://api.sendbridge.com/openapi.json\nschemes:\n  - type: bearer\n    description: API key passed as Bearer token. Prefix `sbk_live_` for production or `sbk_test_` for test.\n"
source_yaml_url: https://artifacts.apis.io/sendbridge-com/authentication/sendbridge-com-authentication.yml
summary_line: 1 scheme
tags:
- email
- verification
- api
- deliverability
- validation
- marketing
- service
---
