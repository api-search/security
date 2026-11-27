---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zvonok-default-api-openapi.yml
  format: yaml
  label: Zvonok Абонентские номера API
  slug: zvonok-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvonok/openapi/zvonok-default-api-openapi.yml
- filename: zvonok-sip-api-openapi.yml
  format: yaml
  label: Zvonok SIP Линии API
  slug: zvonok-sip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvonok/openapi/zvonok-sip-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Zvonok Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zvonok secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Zvonok
provider_slug: zvonok
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/zvonok-openapi.json
  type: http
slug: zvonok-authentication
source_filename: zvonok-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: derived\nsource: openapi/zvonok-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/zvonok-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/zvonok/authentication/zvonok-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Telephony
- Automation
- Artificial Intelligence
- Marketing
- Sales
---
