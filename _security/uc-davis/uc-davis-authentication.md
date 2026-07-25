---
api_key_in:
- header
api_specs:
- filename: uc-davis-access-api-openapi.yml
  format: yaml
  label: University of California, Davis Access API
  slug: uc-davis-access-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-access-api-openapi.yml
- filename: uc-davis-documents-api-openapi.yml
  format: yaml
  label: University of California, Davis Documents API
  slug: uc-davis-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-documents-api-openapi.yml
- filename: uc-davis-equipment-api-openapi.yml
  format: yaml
  label: University of California, Davis Equipment API
  slug: uc-davis-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-equipment-api-openapi.yml
- filename: uc-davis-keys-api-openapi.yml
  format: yaml
  label: University of California, Davis Keys API
  slug: uc-davis-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-keys-api-openapi.yml
- filename: uc-davis-keyserials-api-openapi.yml
  format: yaml
  label: University of California, Davis KeySerials API
  slug: uc-davis-keyserials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-keyserials-api-openapi.yml
- filename: uc-davis-people-api-openapi.yml
  format: yaml
  label: University of California, Davis People API
  slug: uc-davis-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-people-api-openapi.yml
- filename: uc-davis-peopleadmin-api-openapi.yml
  format: yaml
  label: University of California, Davis PeopleAdmin API
  slug: uc-davis-peopleadmin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-peopleadmin-api-openapi.yml
- filename: uc-davis-spaces-api-openapi.yml
  format: yaml
  label: University of California, Davis Spaces API
  slug: uc-davis-spaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-spaces-api-openapi.yml
- filename: uc-davis-workstations-api-openapi.yml
  format: yaml
  label: University of California, Davis Workstations API
  slug: uc-davis-workstations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/openapi/uc-davis-workstations-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Uc Davis Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of California, Davis secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of California, Davis
provider_slug: uc-davis
scheme_count: 1
schemes:
- description: API Key Authentication
  in: header
  name: ApiKey
  parameter: X-Auth-Token
  sources:
  - openapi/uc-davis-peaks.yaml
  type: apiKey
slug: uc-davis-authentication
source_filename: uc-davis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/uc-davis-peaks.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: X-Auth-Token\n  description: API Key Authentication\n  sources:\n  - openapi/uc-davis-peaks.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uc-davis/refs/heads/main/authentication/uc-davis-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- United States
- California
- Identity
- Health
---
