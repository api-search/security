---
api_key_in:
- query
api_specs:
- filename: comeet-careers-api-openapi.yml
  format: yaml
  label: Comeet Careers API
  slug: comeet-careers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/comeet/refs/heads/main/openapi/comeet-careers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Comeet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Comeet secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Comeet
provider_slug: comeet
scheme_count: 1
schemes:
- description: Public company token issued by Comeet for the Careers API.
  in: query
  name: companyToken
  parameter: token
  sources:
  - openapi/comeet-careers-api-openapi.yml
  type: apiKey
slug: comeet-authentication
source_filename: comeet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/comeet-careers-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: companyToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: Public company token issued by Comeet for the Careers API.\n  sources:\n  - openapi/comeet-careers-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/comeet/refs/heads/main/authentication/comeet-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ATS
- Candidates
- Careers
- Interviews
- Jobs
- Recruiting
- Talent Acquisition
---
