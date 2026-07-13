---
api_key_in:
- header
api_specs:
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Jobs API
  slug: jobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Applications API
  slug: applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Applicants API
  slug: applicants
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Job Stages API
  slug: job-stages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Comments and Files API
  slug: comments-files
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
- filename: pinpoint-openapi.yml
  format: yaml
  label: Pinpoint Webhooks
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/openapi/pinpoint-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pinpoint Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pinpoint secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Pinpoint
provider_slug: pinpoint
scheme_count: 1
schemes:
- description: API key generated in Settings > API & Webhooks > API Keys. Sent with every request as the X-API-KEY header. Missing or invalid keys return HTTP 401.
  in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/pinpoint-openapi.yml
  type: apiKey
slug: pinpoint-authentication
source_filename: pinpoint-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pinpoint-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  description: API key generated in Settings > API & Webhooks > API Keys. Sent with every request\n    as the X-API-KEY header. Missing or invalid keys return HTTP 401.\n  sources:\n  - openapi/pinpoint-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pinpoint/refs/heads/main/authentication/pinpoint-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- ATS
- Recruitment
- Hiring
- HR Tech
- JSON:API
---
