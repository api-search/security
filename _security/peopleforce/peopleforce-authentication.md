---
api_key_in: []
api_specs:
- filename: peopleforce-candidates-api-openapi.yml
  format: yaml
  label: PeopleForce Candidates API
  slug: peopleforce-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/openapi/peopleforce-candidates-api-openapi.yml
- filename: peopleforce-departments-api-openapi.yml
  format: yaml
  label: PeopleForce Departments API
  slug: peopleforce-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/openapi/peopleforce-departments-api-openapi.yml
- filename: peopleforce-divisions-api-openapi.yml
  format: yaml
  label: PeopleForce Divisions API
  slug: peopleforce-divisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/openapi/peopleforce-divisions-api-openapi.yml
- filename: peopleforce-employees-api-openapi.yml
  format: yaml
  label: PeopleForce Employees API
  slug: peopleforce-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/openapi/peopleforce-employees-api-openapi.yml
- filename: peopleforce-leave-requests-api-openapi.yml
  format: yaml
  label: PeopleForce Leave Requests API
  slug: peopleforce-leave-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/openapi/peopleforce-leave-requests-api-openapi.yml
- filename: peopleforce-positions-api-openapi.yml
  format: yaml
  label: PeopleForce Positions API
  slug: peopleforce-positions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/openapi/peopleforce-positions-api-openapi.yml
- filename: peopleforce-vacancies-api-openapi.yml
  format: yaml
  label: PeopleForce Vacancies API
  slug: peopleforce-vacancies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopleforce/refs/heads/main/openapi/peopleforce-vacancies-api-openapi.yml
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
