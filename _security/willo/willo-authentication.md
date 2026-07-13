---
api_key_in:
- header
api_specs:
- filename: willo-openapi.yml
  format: yaml
  label: Willo Interviews API
  slug: willo-interviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Participants (Candidates) API
  slug: willo-participants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Departments API
  slug: willo-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Webhooks API
  slug: willo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Message Templates API
  slug: willo-message-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Users API
  slug: willo-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Interview Templates API
  slug: willo-interview-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
- filename: willo-openapi.yml
  format: yaml
  label: Willo Child Organisations API
  slug: willo-child-organisations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/openapi/willo-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Willo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Willo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Willo
provider_slug: willo
scheme_count: 1
schemes:
- description: The integration key ("API key") available on the Willo Integrations page at https://app.willotalent.com/integrations, sent in the Authorization header. Each user has their own key carrying that user's permissions.
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/willo-openapi.yml
  type: apiKey
slug: willo-authentication
source_filename: willo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/willo-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: The integration key (\"API key\") available on the Willo Integrations page at https://app.willotalent.com/integrations,\n    sent in the Authorization header. Each user has their own key carrying that user's permissions.\n  sources:\n  - openapi/willo-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/willo/refs/heads/main/authentication/willo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Video Interviewing
- Recruitment
- HR Tech
- ATS
- Screening
- Async Video
---
