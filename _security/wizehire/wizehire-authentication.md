---
anonymous_access: false
api_key_in: []
api_specs:
- filename: wizehire-scout-service-openapi.yml
  format: yaml
  label: Wizehire Scout Service API
  slug: wizehire-scout-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wizehire/refs/heads/main/openapi/wizehire-scout-service-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Wizehire Authentication
name_suffix: Authentication
oauth_flows: []
overview: WizeHire secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WizeHire
provider_slug: wizehire
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/wizehire-scout-service-openapi.yml
  type: http
slug: wizehire-authentication
source_filename: wizehire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: derived\nsource: openapi/wizehire-scout-service-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/wizehire-scout-service-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wizehire/refs/heads/main/authentication/wizehire-authentication.yml
summary_line: http · 1 scheme
tags:
- Hiring
- Recruiting
- Applicant Tracking
- Human Resources
- Talent Assessment
- Small Business
- Artificial Intelligence
- Job Boards
- Onboarding
- HR Tech
---
