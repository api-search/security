---
api_key_in:
- header
api_specs:
- filename: engagedly-activities-api-openapi.yml
  format: yaml
  label: Engagedly Activities API
  slug: engagedly-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/openapi/engagedly-activities-api-openapi.yml
- filename: engagedly-businesses-api-openapi.yml
  format: yaml
  label: Engagedly Businesses API
  slug: engagedly-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/openapi/engagedly-businesses-api-openapi.yml
- filename: engagedly-departments-api-openapi.yml
  format: yaml
  label: Engagedly Departments API
  slug: engagedly-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/openapi/engagedly-departments-api-openapi.yml
- filename: engagedly-job-titles-api-openapi.yml
  format: yaml
  label: Engagedly Job Titles API
  slug: engagedly-job-titles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/openapi/engagedly-job-titles-api-openapi.yml
- filename: engagedly-locations-api-openapi.yml
  format: yaml
  label: Engagedly Locations API
  slug: engagedly-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/openapi/engagedly-locations-api-openapi.yml
- filename: engagedly-permissions-api-openapi.yml
  format: yaml
  label: Engagedly Permissions API
  slug: engagedly-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/openapi/engagedly-permissions-api-openapi.yml
- filename: engagedly-user-attributes-api-openapi.yml
  format: yaml
  label: Engagedly User Attributes API
  slug: engagedly-user-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/openapi/engagedly-user-attributes-api-openapi.yml
- filename: engagedly-users-api-openapi.yml
  format: yaml
  label: Engagedly Users API
  slug: engagedly-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/openapi/engagedly-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Engagedly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Engagedly secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Engagedly
provider_slug: engagedly
scheme_count: 2
schemes:
- description: Client key obtained from the Engagedly portal under Integrations > Engagedly API
  in: header
  name: clientKeyAuth
  parameter: ClientKey
  sources:
  - openapi/engagedly-openapi.yml
  type: apiKey
- description: Secret key obtained from the Engagedly portal. Shown only once upon generation.
  in: header
  name: secretKeyAuth
  parameter: SecretKey
  sources:
  - openapi/engagedly-openapi.yml
  type: apiKey
slug: engagedly-authentication
source_filename: engagedly-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/engagedly-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: clientKeyAuth\n  type: apiKey\n  in: header\n  parameter: ClientKey\n  description: Client key obtained from the Engagedly portal under Integrations > Engagedly\n    API\n  sources:\n  - openapi/engagedly-openapi.yml\n- name: secretKeyAuth\n  type: apiKey\n  in: header\n  parameter: SecretKey\n  description: Secret key obtained from the Engagedly portal. Shown only once upon generation.\n  sources:\n  - openapi/engagedly-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engagedly/refs/heads/main/authentication/engagedly-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Performance Management
- HR Software
- Employee Engagement
- Goal Tracking
- 360 Feedback
- Learning Management
- Employee Recognition
- Talent Management
- OKR
- People Operations
---
