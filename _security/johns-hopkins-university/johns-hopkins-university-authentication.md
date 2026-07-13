---
api_key_in:
- query
api_specs:
- filename: johns-hopkins-university-sis-course-search.yaml
  format: yaml
  label: Self-Service Public Course Search API (SIS)
  slug: sis-course-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/openapi/johns-hopkins-university-sis-course-search.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Johns Hopkins University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Johns Hopkins University secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Johns Hopkins University
provider_slug: johns-hopkins-university
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: key
  sources:
  - openapi/johns-hopkins-university-sis-course-search.yaml
  type: apiKey
slug: johns-hopkins-university-authentication
source_filename: johns-hopkins-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/johns-hopkins-university-sis-course-search.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/johns-hopkins-university-sis-course-search.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/johns-hopkins-university/refs/heads/main/authentication/johns-hopkins-university-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Course Catalog
- News
- United States
---
