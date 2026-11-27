---
anonymous_access: false
api_key_in: []
api_specs:
- filename: switchwize-com-compute-api-openapi.yml
  format: yaml
  label: SwitchWize Compute API
  slug: switchwize-com-compute-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/switchwize-com/openapi/switchwize-com-compute-api-openapi.yml
- filename: switchwize-com-datasets-api-openapi.yml
  format: yaml
  label: SwitchWize Datasets API
  slug: switchwize-com-datasets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/switchwize-com/openapi/switchwize-com-datasets-api-openapi.yml
- filename: switchwize-com-switchwize-data-api-api-openapi.yml
  format: yaml
  label: SwitchWize SwitchWize Data API
  slug: switchwize-com-switchwize-data-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/switchwize-com/openapi/switchwize-com-switchwize-data-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: SwitchWize Authentication
name_suffix: Authentication
oauth_flows: []
overview: SwitchWize secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SwitchWize
provider_slug: switchwize-com
scheme_count: 1
schemes:
- description: API key starting swk_. Also accepted in the X-API-Key header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/switchwize-com-openapi.json
  type: http
slug: switchwize-com-authentication
source_filename: switchwize-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: derived\nsource: openapi/switchwize-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key starting swk_. Also accepted in the X-API-Key header.\n  sources:\n  - openapi/switchwize-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/switchwize-com/authentication/switchwize-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- PersonalFinance
- RateComparison
- Savings
- Mortgages
---
