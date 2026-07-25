---
api_key_in:
- header
api_specs:
- filename: trakstar-auth-api-openapi.yml
  format: yaml
  label: Trakstar Auth API
  slug: trakstar-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-auth-api-openapi.yml
- filename: trakstar-candidate-messages-api-openapi.yml
  format: yaml
  label: Trakstar Candidate Messages API
  slug: trakstar-candidate-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-candidate-messages-api-openapi.yml
- filename: trakstar-candidates-api-openapi.yml
  format: yaml
  label: Trakstar Candidates API
  slug: trakstar-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-candidates-api-openapi.yml
- filename: trakstar-courses-api-openapi.yml
  format: yaml
  label: Trakstar Courses API
  slug: trakstar-courses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-courses-api-openapi.yml
- filename: trakstar-evaluations-api-openapi.yml
  format: yaml
  label: Trakstar Evaluations API
  slug: trakstar-evaluations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-evaluations-api-openapi.yml
- filename: trakstar-groups-api-openapi.yml
  format: yaml
  label: Trakstar Groups API
  slug: trakstar-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-groups-api-openapi.yml
- filename: trakstar-internal-notes-api-openapi.yml
  format: yaml
  label: Trakstar Internal Notes API
  slug: trakstar-internal-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-internal-notes-api-openapi.yml
- filename: trakstar-interviews-api-openapi.yml
  format: yaml
  label: Trakstar Interviews API
  slug: trakstar-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-interviews-api-openapi.yml
- filename: trakstar-openings-api-openapi.yml
  format: yaml
  label: Trakstar Openings API
  slug: trakstar-openings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-openings-api-openapi.yml
- filename: trakstar-reviews-api-openapi.yml
  format: yaml
  label: Trakstar Reviews API
  slug: trakstar-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-reviews-api-openapi.yml
- filename: trakstar-to-dos-api-openapi.yml
  format: yaml
  label: Trakstar To-Dos API
  slug: trakstar-to-dos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-to-dos-api-openapi.yml
- filename: trakstar-users-api-openapi.yml
  format: yaml
  label: Trakstar Users API
  slug: trakstar-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/openapi/trakstar-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trakstar Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trakstar secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Trakstar
provider_slug: trakstar
scheme_count: 2
schemes:
- description: API key generated from the Trakstar Hire Super Admin settings page. Pass as "ApiKey {your_api_key}".
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/trakstar-hire-api-openapi.yml
  type: apiKey
- description: API key provisioned by Trakstar Learn support team. Contact learn@trakstar.com to request access.
  in: header
  name: apiKey
  parameter: x-mindflash-apikey
  sources:
  - openapi/trakstar-learn-api-openapi.yml
  type: apiKey
slug: trakstar-authentication
source_filename: trakstar-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trakstar-hire-api-openapi.yml, openapi/trakstar-learn-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key generated from the Trakstar Hire Super Admin settings page. Pass as \"ApiKey\n    {your_api_key}\".\n  sources:\n  - openapi/trakstar-hire-api-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: x-mindflash-apikey\n  description: API key provisioned by Trakstar Learn support team. Contact learn@trakstar.com\n    to request access.\n  sources:\n  - openapi/trakstar-learn-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trakstar/refs/heads/main/authentication/trakstar-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- HR
- Human Resources
- Performance Management
- Talent Management
- Applicant Tracking
- Learning Management
- 360 Feedback
- Goal Management
- Employee Development
- Performance Appraisal
---
