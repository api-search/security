---
api_key_in:
- query
api_specs:
- filename: department-of-better-technology-files-api-openapi.yml
  format: yaml
  label: Department of Better Technology Files API
  slug: department-of-better-technology-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/openapi/department-of-better-technology-files-api-openapi.yml
- filename: department-of-better-technology-forms-api-openapi.yml
  format: yaml
  label: Department of Better Technology Forms API
  slug: department-of-better-technology-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/openapi/department-of-better-technology-forms-api-openapi.yml
- filename: department-of-better-technology-labels-api-openapi.yml
  format: yaml
  label: Department of Better Technology Labels API
  slug: department-of-better-technology-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/openapi/department-of-better-technology-labels-api-openapi.yml
- filename: department-of-better-technology-projects-api-openapi.yml
  format: yaml
  label: Department of Better Technology Projects API
  slug: department-of-better-technology-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/openapi/department-of-better-technology-projects-api-openapi.yml
- filename: department-of-better-technology-response-assignments-api-openapi.yml
  format: yaml
  label: Department of Better Technology Response Assignments API
  slug: department-of-better-technology-response-assignments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/openapi/department-of-better-technology-response-assignments-api-openapi.yml
- filename: department-of-better-technology-response-labels-api-openapi.yml
  format: yaml
  label: Department of Better Technology Response Labels API
  slug: department-of-better-technology-response-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/openapi/department-of-better-technology-response-labels-api-openapi.yml
- filename: department-of-better-technology-responses-api-openapi.yml
  format: yaml
  label: Department of Better Technology Responses API
  slug: department-of-better-technology-responses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/openapi/department-of-better-technology-responses-api-openapi.yml
- filename: department-of-better-technology-statuses-api-openapi.yml
  format: yaml
  label: Department of Better Technology Statuses API
  slug: department-of-better-technology-statuses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/openapi/department-of-better-technology-statuses-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Department Of Better Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of Better Technology secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Department of Better Technology
provider_slug: department-of-better-technology
scheme_count: 1
schemes:
- description: Your Screendoor API key, obtained in Screendoor under Settings -> API Keys, passed as the `api_key` URL parameter on every request.
  in: query
  name: apiKeyAuth
  parameter: api_key
  sources:
  - openapi/department-of-better-technology-screendoor-openapi.yml
  type: apiKey
slug: department-of-better-technology-authentication
source_filename: department-of-better-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/department-of-better-technology-screendoor-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Your Screendoor API key, obtained in Screendoor under Settings -> API Keys, passed\n    as the `api_key` URL parameter on every request.\n  sources:\n  - openapi/department-of-better-technology-screendoor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-better-technology/refs/heads/main/authentication/department-of-better-technology-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Forms
- Government
- GovTech
- Civic Technology
- Workflow
- Data Collection
- Screendoor
- Public Sector
- Forms API
---
