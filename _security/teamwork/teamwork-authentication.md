---
api_key_in: []
api_specs:
- filename: download
  format: yaml
  label: Teamwork.com Projects API v3
  slug: projects-api-v3
  spec_type: OpenAPI
  url: https://apidocs.teamwork.com/api/oas/download?slug=teamwork&api_version=v3
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Teamwork Authentication
name_suffix: Authentication
oauth_flows: []
overview: Teamwork.com secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Teamwork.com
provider_slug: teamwork
scheme_count: 2
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/teamwork-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/teamwork-openapi.yml
  type: http
slug: teamwork-authentication
source_filename: teamwork-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/teamwork-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/teamwork-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/teamwork-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teamwork/refs/heads/main/authentication/teamwork-authentication.yml
summary_line: http · 2 schemes
tags:
- Project Management
- Client Services
- Task Management
- Time Tracking
- Collaboration
- Professional Services Automation
---
