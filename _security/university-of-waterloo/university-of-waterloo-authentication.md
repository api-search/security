---
api_key_in:
- header
api_specs:
- filename: university-of-waterloo-academicorganizations-api-openapi.yml
  format: yaml
  label: University of Waterloo AcademicOrganizations API
  slug: university-of-waterloo-academicorganizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-academicorganizations-api-openapi.yml
- filename: university-of-waterloo-account-api-openapi.yml
  format: yaml
  label: University of Waterloo Account API
  slug: university-of-waterloo-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-account-api-openapi.yml
- filename: university-of-waterloo-classschedules-api-openapi.yml
  format: yaml
  label: University of Waterloo ClassSchedules API
  slug: university-of-waterloo-classschedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-classschedules-api-openapi.yml
- filename: university-of-waterloo-courses-api-openapi.yml
  format: yaml
  label: University of Waterloo Courses API
  slug: university-of-waterloo-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-courses-api-openapi.yml
- filename: university-of-waterloo-examschedules-api-openapi.yml
  format: yaml
  label: University of Waterloo ExamSchedules API
  slug: university-of-waterloo-examschedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-examschedules-api-openapi.yml
- filename: university-of-waterloo-foodservices-api-openapi.yml
  format: yaml
  label: University of Waterloo FoodServices API
  slug: university-of-waterloo-foodservices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-foodservices-api-openapi.yml
- filename: university-of-waterloo-holidaydates-api-openapi.yml
  format: yaml
  label: University of Waterloo HolidayDates API
  slug: university-of-waterloo-holidaydates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-holidaydates-api-openapi.yml
- filename: university-of-waterloo-importantdates-api-openapi.yml
  format: yaml
  label: University of Waterloo ImportantDates API
  slug: university-of-waterloo-importantdates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-importantdates-api-openapi.yml
- filename: university-of-waterloo-locations-api-openapi.yml
  format: yaml
  label: University of Waterloo Locations API
  slug: university-of-waterloo-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-locations-api-openapi.yml
- filename: university-of-waterloo-subjects-api-openapi.yml
  format: yaml
  label: University of Waterloo Subjects API
  slug: university-of-waterloo-subjects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-subjects-api-openapi.yml
- filename: university-of-waterloo-terms-api-openapi.yml
  format: yaml
  label: University of Waterloo Terms API
  slug: university-of-waterloo-terms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-terms-api-openapi.yml
- filename: university-of-waterloo-wcms-api-openapi.yml
  format: yaml
  label: University of Waterloo Wcms API
  slug: university-of-waterloo-wcms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/openapi/university-of-waterloo-wcms-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: University Of Waterloo Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Waterloo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Waterloo
provider_slug: university-of-waterloo
scheme_count: 1
schemes:
- description: Custom API key authentication
  in: header
  name: apiKey
  parameter: x-api-key
  sources:
  - openapi/_original/university-of-waterloo-open-data-api.yaml
  type: apiKey
slug: university-of-waterloo-authentication
source_filename: university-of-waterloo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/_original/university-of-waterloo-open-data-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: Custom API key authentication\n  sources:\n  - openapi/_original/university-of-waterloo-open-data-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-waterloo/refs/heads/main/authentication/university-of-waterloo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Open Data
- Canada
- Ontario
- Research
- Research Data
- Course Catalog
- Identity Federation
- Research Repository
- Campus Life
---
