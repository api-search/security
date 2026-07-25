---
api_key_in:
- header
api_specs:
- filename: pulse-software-authentication-api-openapi.yml
  format: yaml
  label: Pulse Software Authentication API
  slug: pulse-software-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-authentication-api-openapi.yml
- filename: pulse-software-corporate-planning-api-api-openapi.yml
  format: yaml
  label: Pulse Software Corporate Planning API API
  slug: pulse-software-corporate-planning-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-corporate-planning-api-api-openapi.yml
- filename: pulse-software-forms-api-api-openapi.yml
  format: yaml
  label: Pulse Software Forms API API
  slug: pulse-software-forms-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-forms-api-api-openapi.yml
- filename: pulse-software-learning-api-api-openapi.yml
  format: yaml
  label: Pulse Software Learning API API
  slug: pulse-software-learning-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-learning-api-api-openapi.yml
- filename: pulse-software-project-api-api-openapi.yml
  format: yaml
  label: Pulse Software Project API API
  slug: pulse-software-project-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-project-api-api-openapi.yml
- filename: pulse-software-recruitment-api-api-openapi.yml
  format: yaml
  label: Pulse Software Recruitment API API
  slug: pulse-software-recruitment-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-recruitment-api-api-openapi.yml
- filename: pulse-software-sync-api-api-openapi.yml
  format: yaml
  label: Pulse Software Sync API API
  slug: pulse-software-sync-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-sync-api-api-openapi.yml
- filename: pulse-software-user-details-api-api-openapi.yml
  format: yaml
  label: Pulse Software User Details API API
  slug: pulse-software-user-details-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-user-details-api-api-openapi.yml
- filename: pulse-software-user-details-api-v2-api-openapi.yml
  format: yaml
  label: Pulse Software User Details API v2 API
  slug: pulse-software-user-details-api-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/openapi/pulse-software-user-details-api-v2-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Pulse Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pulse Software secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pulse Software
provider_slug: pulse-software
scheme_count: 2
schemes:
- in: header
  name: ApiKey
  parameter: x-Api-Key
  sources:
  - openapi/pulse-software-openapi.yml
  type: apiKey
- in: header
  name: BearerJWT
  parameter: Authorisation
  sources:
  - openapi/pulse-software-openapi.yml
  type: apiKey
slug: pulse-software-authentication
source_filename: pulse-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pulse-software-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-Api-Key\n  sources:\n  - openapi/pulse-software-openapi.yml\n- name: BearerJWT\n  type: apiKey\n  in: header\n  parameter: Authorisation\n  sources:\n  - openapi/pulse-software-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pulse-software/refs/heads/main/authentication/pulse-software-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Pulse
- Automation
- Developer
---
