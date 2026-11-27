---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: kindwise-com-health-assessment-api-openapi.yml
  format: yaml
  label: Kindwise Health Assessment API
  slug: kindwise-com-health-assessment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kindwise-com/openapi/kindwise-com-health-assessment-api-openapi.yml
- filename: kindwise-com-identification-api-openapi.yml
  format: yaml
  label: Kindwise Identification API
  slug: kindwise-com-identification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kindwise-com/openapi/kindwise-com-identification-api-openapi.yml
- filename: kindwise-com-kb-api-openapi.yml
  format: yaml
  label: Kindwise Kb API
  slug: kindwise-com-kb-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kindwise-com/openapi/kindwise-com-kb-api-openapi.yml
- filename: kindwise-com-usage-info-api-openapi.yml
  format: yaml
  label: Kindwise Usage Info API
  slug: kindwise-com-usage-info-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kindwise-com/openapi/kindwise-com-usage-info-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Kindwise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kindwise secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kindwise
provider_slug: kindwise-com
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: Api-Key
  sources:
  - openapi/kindwise-com-openapi.yaml
  type: apiKey
slug: kindwise-com-authentication
source_filename: kindwise-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/kindwise-com-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  sources:\n  - openapi/kindwise-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/kindwise-com/authentication/kindwise-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Identification
- Plant
- Insect
- Mushroom
- Agriculture
---
