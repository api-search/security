---
anonymous_access: false
api_key_in: []
api_specs:
- filename: buzzmebro-com-applications-api-openapi.yml
  format: yaml
  label: BuzzMeBro Applications API
  slug: buzzmebro-com-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-applications-api-openapi.yml
- filename: buzzmebro-com-check-api-openapi.yml
  format: yaml
  label: BuzzMeBro Check API
  slug: buzzmebro-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-check-api-openapi.yml
- filename: buzzmebro-com-info-api-openapi.yml
  format: yaml
  label: BuzzMeBro Info API
  slug: buzzmebro-com-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-info-api-openapi.yml
- filename: buzzmebro-com-me-api-openapi.yml
  format: yaml
  label: BuzzMeBro Me API
  slug: buzzmebro-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-me-api-openapi.yml
- filename: buzzmebro-com-setups-api-openapi.yml
  format: yaml
  label: BuzzMeBro Setups API
  slug: buzzmebro-com-setups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buzzmebro-com/openapi/buzzmebro-com-setups-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Buzzmebro Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BuzzMeBro secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BuzzMeBro
provider_slug: buzzmebro-com
scheme_count: 1
schemes:
- description: status_token from createSetup.
  name: statusToken
  scheme: bearer
  sources:
  - openapi/buzzmebro-com-agent-openapi.json
  - openapi/buzzmebro-com-partner-openapi.json
  type: http
slug: buzzmebro-com-authentication
source_filename: buzzmebro-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: derived\nsource: openapi/buzzmebro-com-agent-openapi.json, openapi/buzzmebro-com-partner-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: statusToken\n  type: http\n  scheme: bearer\n  description: status_token from createSetup.\n  sources:\n  - openapi/buzzmebro-com-agent-openapi.json\n  - openapi/buzzmebro-com-partner-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/buzzmebro-com/authentication/buzzmebro-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Buzzer
- Apartments
- Access
- Subscription
- Toronto
---
