---
api_key_in:
- header
api_specs:
- filename: regulations-gov-comment-submission-utilities-api-openapi.yml
  format: yaml
  label: Regulations.gov comment submission utilities API
  slug: regulations-gov-comment-submission-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regulations-gov/refs/heads/main/openapi/regulations-gov-comment-submission-utilities-api-openapi.yml
- filename: regulations-gov-comments-api-openapi.yml
  format: yaml
  label: Regulations.gov comments API
  slug: regulations-gov-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regulations-gov/refs/heads/main/openapi/regulations-gov-comments-api-openapi.yml
- filename: regulations-gov-dockets-api-openapi.yml
  format: yaml
  label: Regulations.gov dockets API
  slug: regulations-gov-dockets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regulations-gov/refs/heads/main/openapi/regulations-gov-dockets-api-openapi.yml
- filename: regulations-gov-documents-api-openapi.yml
  format: yaml
  label: Regulations.gov documents API
  slug: regulations-gov-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regulations-gov/refs/heads/main/openapi/regulations-gov-documents-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Regulations Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Regulations.gov secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Regulations.gov
provider_slug: regulations-gov
scheme_count: 1
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/regulations-gov-regulations-gov-api-openapi.yml
  type: apiKey
slug: regulations-gov-authentication
source_filename: regulations-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/regulations-gov-regulations-gov-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/regulations-gov-regulations-gov-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regulations-gov/refs/heads/main/authentication/regulations-gov-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Federal Rulemaking
- Public Comments
- Regulatory
- Dockets
- GSA
- Open Data
---
