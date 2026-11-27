---
anonymous_access: false
api_key_in: []
api_specs:
- filename: intakra-com-accounts-api-openapi.yml
  format: yaml
  label: Intakra Accounts API
  slug: intakra-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intakra-com/openapi/intakra-com-accounts-api-openapi.yml
- filename: intakra-com-brief-api-openapi.yml
  format: yaml
  label: Intakra Brief API
  slug: intakra-com-brief-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intakra-com/openapi/intakra-com-brief-api-openapi.yml
- filename: intakra-com-opportunities-api-openapi.yml
  format: yaml
  label: Intakra Opportunities API
  slug: intakra-com-opportunities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intakra-com/openapi/intakra-com-opportunities-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Intakra Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intakra secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Intakra
provider_slug: intakra-com
scheme_count: 1
schemes:
- description: A workspace API key (ik_live_...). A workspace member creates it in Settings, API and MCP; it is shown once and can be revoked there.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/intakra-com-openapi.json
  type: http
slug: intakra-com-authentication
source_filename: intakra-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/intakra-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: A workspace API key (ik_live_...). A workspace member creates it in Settings,\n    API and MCP; it is shown once and can be revoked there.\n  sources:\n  - openapi/intakra-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/intakra-com/authentication/intakra-com-authentication.yml
summary_line: http · 1 scheme
tags:
- B2B
- Sales
- Marketing
- AccountMonitoring
- Buying Signals
---
