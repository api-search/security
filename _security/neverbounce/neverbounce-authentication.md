---
api_key_in:
- query
api_specs:
- filename: neverbounce-openapi.yml
  format: yaml
  label: NeverBounce API v4
  slug: v4-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/openapi/neverbounce-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Neverbounce Authentication
name_suffix: Authentication
oauth_flows: []
overview: NeverBounce secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NeverBounce
provider_slug: neverbounce
scheme_count: 2
schemes:
- in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/neverbounce-openapi.yml
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/neverbounce-openapi.yml
  type: http
slug: neverbounce-authentication
source_filename: neverbounce-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/neverbounce-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  sources:\n  - openapi/neverbounce-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/neverbounce-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/neverbounce/refs/heads/main/authentication/neverbounce-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Email Verification
- Email Validation
- Email Hygiene
- Deliverability
- Marketing
- List Cleaning
- ZeroBounce
---
