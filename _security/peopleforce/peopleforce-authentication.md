---
api_key_in: []
api_specs:
- filename: peopleforce-openapi.yml
  format: yaml
  label: PeopleForce API
  slug: peopleforce
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/openapi/peopleforce-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Peopleforce Authentication
name_suffix: Authentication
oauth_flows: []
overview: PeopleForce secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PeopleForce
provider_slug: peopleforce
scheme_count: 1
schemes:
- bearerFormat: API Token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/peopleforce-openapi.yml
  type: http
slug: peopleforce-authentication
source_filename: peopleforce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/peopleforce-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: API Token\n  sources:\n  - openapi/peopleforce-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/authentication/peopleforce-authentication.yml
summary_line: http · 1 scheme
tags:
- HR
- Human Resources
- Recruitment
- Employees
---
