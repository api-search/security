---
api_key_in: []
api_specs:
- filename: careacademy-compliance-report-api-openapi.yml
  format: yaml
  label: CareAcademy Compliance Report API
  slug: careacademy-compliance-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/careacademy/refs/heads/main/openapi/careacademy-compliance-report-api-openapi.yml
- filename: careacademy-locations-api-openapi.yml
  format: yaml
  label: CareAcademy Locations API
  slug: careacademy-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/careacademy/refs/heads/main/openapi/careacademy-locations-api-openapi.yml
- filename: careacademy-organizations-api-openapi.yml
  format: yaml
  label: CareAcademy Organizations API
  slug: careacademy-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/careacademy/refs/heads/main/openapi/careacademy-organizations-api-openapi.yml
- filename: careacademy-practitioners-api-openapi.yml
  format: yaml
  label: CareAcademy Practitioners API
  slug: careacademy-practitioners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/careacademy/refs/heads/main/openapi/careacademy-practitioners-api-openapi.yml
- filename: careacademy-sign-in-url-api-openapi.yml
  format: yaml
  label: CareAcademy Sign In Url API
  slug: careacademy-sign-in-url-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/careacademy/refs/heads/main/openapi/careacademy-sign-in-url-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Careacademy Authentication
name_suffix: Authentication
oauth_flows: []
overview: CareAcademy secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CareAcademy
provider_slug: careacademy
scheme_count: 1
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/careacademy-openapi-original.yml
  type: http
slug: careacademy-authentication
source_filename: careacademy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/careacademy-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/careacademy-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/careacademy/refs/heads/main/authentication/careacademy-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Training
- Education
- Compliance
- Home Care
- Home Health
- Hospice
- Senior Living
- Healthcare
- Workforce Management
- Single Sign-On
- Caregivers
---
