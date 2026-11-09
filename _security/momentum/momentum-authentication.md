---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: momentum-openapi-generated.yml
  format: yaml
  label: Momentum API
  slug: momentum-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/momentum/openapi/_ae-authored/momentum-openapi-generated.yml
- filename: momentum-meeting-api-openapi.yml
  format: yaml
  label: Momentum Meeting API
  slug: momentum-meeting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/momentum/openapi/momentum-meeting-api-openapi.yml
- filename: momentum-momentum-api-api-openapi.yml
  format: yaml
  label: Momentum Momentum API
  slug: momentum-momentum-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/momentum/openapi/momentum-momentum-api-api-openapi.yml
- filename: momentum-signals-api-openapi.yml
  format: yaml
  label: Momentum Signals API
  slug: momentum-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/momentum/openapi/momentum-signals-api-openapi.yml
- filename: momentum-user-provided-meeting-api-openapi.yml
  format: yaml
  label: Momentum User Provided Meeting API
  slug: momentum-user-provided-meeting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/momentum/openapi/momentum-user-provided-meeting-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Momentum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Momentum secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Momentum
provider_slug: momentum
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-API-Key
  sources:
  - openapi/momentum-meeting-api-openapi.yml
  - openapi/momentum-momentum-api-api-openapi.yml
  - openapi/momentum-signals-api-openapi.yml
  - openapi/momentum-user-provided-meeting-api-openapi.yml
  type: apiKey
slug: momentum-authentication
source_filename: momentum-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/momentum-meeting-api-openapi.yml, openapi/momentum-momentum-api-api-openapi.yml,\n  openapi/momentum-signals-api-openapi.yml, openapi/momentum-user-provided-meeting-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/momentum-meeting-api-openapi.yml\n  - openapi/momentum-momentum-api-api-openapi.yml\n  - openapi/momentum-signals-api-openapi.yml\n  - openapi/momentum-user-provided-meeting-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/momentum/authentication/momentum-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Revenue
- Automation
- Salesforce
---
