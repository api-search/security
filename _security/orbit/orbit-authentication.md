---
api_key_in:
- query
api_specs:
- filename: orbit-activities-api-openapi.yml
  format: yaml
  label: Orbit Activities API
  slug: orbit-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/openapi/orbit-activities-api-openapi.yml
- filename: orbit-activity-types-api-openapi.yml
  format: yaml
  label: Orbit Activity Types API
  slug: orbit-activity-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/openapi/orbit-activity-types-api-openapi.yml
- filename: orbit-members-api-openapi.yml
  format: yaml
  label: Orbit Members API
  slug: orbit-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/openapi/orbit-members-api-openapi.yml
- filename: orbit-notes-api-openapi.yml
  format: yaml
  label: Orbit Notes API
  slug: orbit-notes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/openapi/orbit-notes-api-openapi.yml
- filename: orbit-organizations-api-openapi.yml
  format: yaml
  label: Orbit Organizations API
  slug: orbit-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/openapi/orbit-organizations-api-openapi.yml
- filename: orbit-reports-api-openapi.yml
  format: yaml
  label: Orbit Reports API
  slug: orbit-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/openapi/orbit-reports-api-openapi.yml
- filename: orbit-users-api-openapi.yml
  format: yaml
  label: Orbit Users API
  slug: orbit-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/openapi/orbit-users-api-openapi.yml
- filename: orbit-webhooks-api-openapi.yml
  format: yaml
  label: Orbit Webhooks API
  slug: orbit-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/openapi/orbit-webhooks-api-openapi.yml
- filename: orbit-workspaces-api-openapi.yml
  format: yaml
  label: Orbit Workspaces API
  slug: orbit-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/openapi/orbit-workspaces-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Orbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Orbit secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Orbit
provider_slug: orbit
scheme_count: 2
schemes:
- description: Provide a Authorization header with format 'Bearer <api_key>'. This is the recommended approach. Make sure to include the 'Bearer' part in the text box here.
  name: bearer
  scheme: bearer
  sources:
  - openapi/orbit-rest-api-openapi.yml
  type: http
- description: Provide the API key in a query param called api_key. This is the least secure method, please use only for testing.
  in: query
  name: api_key
  parameter: api_key
  sources:
  - openapi/orbit-rest-api-openapi.yml
  type: apiKey
slug: orbit-authentication
source_filename: orbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/orbit-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  description: Provide a Authorization header with format 'Bearer <api_key>'. This is the recommended\n    approach. Make sure to include the 'Bearer' part in the text box here.\n  sources:\n  - openapi/orbit-rest-api-openapi.yml\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Provide the API key in a query param called api_key. This is the least secure\n    method, please use only for testing.\n  sources:\n  - openapi/orbit-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbit/refs/heads/main/authentication/orbit-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Developer Relations
- Community Intelligence
- DevRel
- Community Management
- Member Tracking
- Community Analytics
- Open Source
- Developer Engagement
---
