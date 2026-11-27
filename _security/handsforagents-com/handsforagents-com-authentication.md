---
anonymous_access: false
api_key_in: []
api_specs:
- filename: handsforagents-com-pay-api-openapi.yml
  format: yaml
  label: Hands for Agents Pay API
  slug: handsforagents-com-pay-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handsforagents-com/openapi/handsforagents-com-pay-api-openapi.yml
- filename: handsforagents-com-quotes-api-openapi.yml
  format: yaml
  label: Hands for Agents Quotes API
  slug: handsforagents-com-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handsforagents-com/openapi/handsforagents-com-quotes-api-openapi.yml
- filename: handsforagents-com-services-api-openapi.yml
  format: yaml
  label: Hands for Agents Services API
  slug: handsforagents-com-services-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handsforagents-com/openapi/handsforagents-com-services-api-openapi.yml
- filename: handsforagents-com-tasks-api-openapi.yml
  format: yaml
  label: Hands for Agents Tasks API
  slug: handsforagents-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handsforagents-com/openapi/handsforagents-com-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Hands for Agents Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hands for Agents secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hands for Agents
provider_slug: handsforagents-com
scheme_count: 1
schemes:
- description: access_token returned by POST /quotes. Valid for that quote and the task created from it.
  name: taskToken
  scheme: bearer
  sources:
  - openapi/handsforagents-com-openapi.yaml
  type: http
slug: handsforagents-com-authentication
source_filename: handsforagents-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-11'\nmethod: derived\nsource: openapi/handsforagents-com-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: taskToken\n  type: http\n  scheme: bearer\n  description: access_token returned by POST /quotes. Valid for that quote and the task created\n    from it.\n  sources:\n  - openapi/handsforagents-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/handsforagents-com/authentication/handsforagents-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Engineering
- Physical-World
- Czech Republic
- Services
---
