---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: recruitee-c-api-openapi.yml
  format: yaml
  label: Recruitee C API
  slug: recruitee-c-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/openapi/recruitee-c-api-openapi.yml
- filename: recruitee-i-api-openapi.yml
  format: yaml
  label: Recruitee I API
  slug: recruitee-i-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/openapi/recruitee-i-api-openapi.yml
- filename: recruitee-offers-api-openapi.yml
  format: yaml
  label: Recruitee Offers API
  slug: recruitee-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/openapi/recruitee-offers-api-openapi.yml
- filename: recruitee-p-api-openapi.yml
  format: yaml
  label: Recruitee P API
  slug: recruitee-p-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/openapi/recruitee-p-api-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Recruitee Authentication
name_suffix: Authentication
oauth_flows: []
overview: Recruitee secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Recruitee
provider_slug: recruitee
scheme_count: 2
schemes:
- flows: []
  name: sec0
  sources:
  - openapi/recruitee-ats-api-openapi.yml
  - openapi/recruitee-partners-release-candidate-token-openapi.yml
  type: oauth2
- in: header
  name: sec0
  parameter: RT-PARTNER-SECRET
  sources:
  - openapi/recruitee-partners-production-secret-openapi.yml
  - openapi/recruitee-partners-release-candidate-secret-openapi.yml
  type: apiKey
slug: recruitee-authentication
source_filename: recruitee-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: derived\nsource: openapi/recruitee-ats-api-openapi.yml, openapi/recruitee-partners-production-secret-openapi.yml,\n  openapi/recruitee-partners-release-candidate-secret-openapi.yml, openapi/recruitee-partners-release-candidate-token-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\nschemes:\n- name: sec0\n  type: oauth2\n  flows: []\n  sources:\n  - openapi/recruitee-ats-api-openapi.yml\n  - openapi/recruitee-partners-release-candidate-token-openapi.yml\n- name: sec0\n  type: apiKey\n  in: header\n  parameter: RT-PARTNER-SECRET\n  sources:\n  - openapi/recruitee-partners-production-secret-openapi.yml\n  - openapi/recruitee-partners-release-candidate-secret-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/recruitee/refs/heads/main/authentication/recruitee-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Recruiting
- Applicant Tracking
- Human Resources
- Hiring
- Careers Site
- Tellent
---
