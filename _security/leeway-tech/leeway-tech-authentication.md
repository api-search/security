---
anonymous_access: false
api_key_in:
- query
api_specs:
- filename: leeway-tech-public-api-openapi.yml
  format: yaml
  label: Leeway Public API
  slug: leeway-tech-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leeway-tech/openapi/leeway-tech-public-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Leeway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leeway secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Leeway
provider_slug: leeway-tech
scheme_count: 1
schemes:
- in: query
  name: apiTokenAuth
  parameter: apitoken
  sources:
  - openapi/leeway-tech-openapi.json
  type: apiKey
slug: leeway-tech-authentication
source_filename: leeway-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: derived\nsource: openapi/leeway-tech-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiTokenAuth\n  type: apiKey\n  in: query\n  parameter: apitoken\n  sources:\n  - openapi/leeway-tech-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/leeway-tech/authentication/leeway-tech-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Finance
- Stock Analysis
- Market Research
---
