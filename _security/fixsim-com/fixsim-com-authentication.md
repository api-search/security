---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: fixsim-com-executionsin-api-openapi.yml
  format: yaml
  label: FIXSIM Executions In API
  slug: fixsim-com-executionsin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-executionsin-api-openapi.yml
- filename: fixsim-com-executionsout-api-openapi.yml
  format: yaml
  label: FIXSIM Executions Out API
  slug: fixsim-com-executionsout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-executionsout-api-openapi.yml
- filename: fixsim-com-instances-api-openapi.yml
  format: yaml
  label: FIXSIM Instances API
  slug: fixsim-com-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-instances-api-openapi.yml
- filename: fixsim-com-ordersin-api-openapi.yml
  format: yaml
  label: FIXSIM Orders In API
  slug: fixsim-com-ordersin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-ordersin-api-openapi.yml
- filename: fixsim-com-ordersout-api-openapi.yml
  format: yaml
  label: FIXSIM Orders Out API
  slug: fixsim-com-ordersout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-ordersout-api-openapi.yml
- filename: fixsim-com-rawmessages-api-openapi.yml
  format: yaml
  label: FIXSIM Raw Messages API
  slug: fixsim-com-rawmessages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-rawmessages-api-openapi.yml
- filename: fixsim-com-securities-api-openapi.yml
  format: yaml
  label: FIXSIM Securities API
  slug: fixsim-com-securities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-securities-api-openapi.yml
- filename: fixsim-com-sessions-api-openapi.yml
  format: yaml
  label: FIXSIM Sessions API
  slug: fixsim-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-sessions-api-openapi.yml
- filename: fixsim-com-sessionsettings-api-openapi.yml
  format: yaml
  label: FIXSIM Session Settings API
  slug: fixsim-com-sessionsettings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-sessionsettings-api-openapi.yml
- filename: fixsim-com-sso-api-openapi.yml
  format: yaml
  label: FIXSIM SSO API
  slug: fixsim-com-sso-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fixsim-com/openapi/fixsim-com-sso-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: FIXSIM Authentication
name_suffix: Authentication
oauth_flows: []
overview: FIXSIM secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FIXSIM
provider_slug: fixsim-com
scheme_count: 1
schemes:
- description: API Key Authentication
  in: header
  name: ApiKey
  parameter: apiKey
  sources:
  - openapi/fixsim-com-openapi.json
  - openapi/portal.fixsim.com.swagger.json
  type: apiKey
slug: fixsim-com-authentication
source_filename: fixsim-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/fixsim-com-openapi.json, openapi/portal.fixsim.com.swagger.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: apiKey\n  description: API Key Authentication\n  sources:\n  - openapi/fixsim-com-openapi.json\n  - openapi/portal.fixsim.com.swagger.json\n"
source_yaml_url: https://artifacts.apis.io/fixsim-com/authentication/fixsim-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- FIX
- FIX Protocol
- Testing
- Sandbox
- Financial Services
---
