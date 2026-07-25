---
api_key_in:
- header
api_specs:
- filename: breeze-chms-account-api-openapi.yml
  format: yaml
  label: Breeze ChMS Account API
  slug: breeze-chms-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-account-api-openapi.yml
- filename: breeze-chms-attendance-api-openapi.yml
  format: yaml
  label: Breeze ChMS Attendance API
  slug: breeze-chms-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-attendance-api-openapi.yml
- filename: breeze-chms-events-api-openapi.yml
  format: yaml
  label: Breeze ChMS Events API
  slug: breeze-chms-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-events-api-openapi.yml
- filename: breeze-chms-forms-api-openapi.yml
  format: yaml
  label: Breeze ChMS Forms API
  slug: breeze-chms-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-forms-api-openapi.yml
- filename: breeze-chms-funds-api-openapi.yml
  format: yaml
  label: Breeze ChMS Funds API
  slug: breeze-chms-funds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-funds-api-openapi.yml
- filename: breeze-chms-giving-api-openapi.yml
  format: yaml
  label: Breeze ChMS Giving API
  slug: breeze-chms-giving-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-giving-api-openapi.yml
- filename: breeze-chms-people-api-openapi.yml
  format: yaml
  label: Breeze ChMS People API
  slug: breeze-chms-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-people-api-openapi.yml
- filename: breeze-chms-pledges-api-openapi.yml
  format: yaml
  label: Breeze ChMS Pledges API
  slug: breeze-chms-pledges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-pledges-api-openapi.yml
- filename: breeze-chms-tags-api-openapi.yml
  format: yaml
  label: Breeze ChMS Tags API
  slug: breeze-chms-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-tags-api-openapi.yml
- filename: breeze-chms-volunteers-api-openapi.yml
  format: yaml
  label: Breeze ChMS Volunteers API
  slug: breeze-chms-volunteers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/openapi/breeze-chms-volunteers-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Breeze Chms Authentication
name_suffix: Authentication
oauth_flows: []
overview: Breeze ChMS secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Breeze ChMS
provider_slug: breeze-chms
scheme_count: 1
schemes:
- description: Account API key sent in the Api-Key header. The Account Owner generates it under Manage Account > API Key in the Breeze web app.
  in: header
  name: apiKeyAuth
  parameter: Api-Key
  sources:
  - openapi/breeze-chms-openapi.yml
  type: apiKey
slug: breeze-chms-authentication
source_filename: breeze-chms-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/breeze-chms-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Account API key sent in the Api-Key header. The Account Owner generates it under\n    Manage Account > API Key in the Breeze web app.\n  sources:\n  - openapi/breeze-chms-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breeze-chms/refs/heads/main/authentication/breeze-chms-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Church Management
- ChMS
- Nonprofit
- Giving
- Membership
- Events
- Faith
---
