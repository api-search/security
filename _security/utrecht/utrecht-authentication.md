---
api_key_in:
- cookie
api_specs:
- filename: utrecht-yoda-core.yaml
  format: yaml
  label: Yoda Research Data Management Platform
  slug: yoda
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/openapi/utrecht-yoda-core.yaml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Utrecht Authentication
name_suffix: Authentication
oauth_flows: []
overview: Utrecht University secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Utrecht University
provider_slug: utrecht
scheme_count: 2
schemes:
- in: cookie
  name: cookieAuth
  parameter: yoda_session
  sources:
  - openapi/utrecht-yoda-core.yaml
  - openapi/utrecht-yoda-datarequest.yaml
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/utrecht-yoda-core.yaml
  - openapi/utrecht-yoda-datarequest.yaml
  type: http
slug: utrecht-authentication
source_filename: utrecht-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/utrecht-yoda-core.yaml, openapi/utrecht-yoda-datarequest.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: yoda_session\n  sources:\n  - openapi/utrecht-yoda-core.yaml\n  - openapi/utrecht-yoda-datarequest.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/utrecht-yoda-core.yaml\n  - openapi/utrecht-yoda-datarequest.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/utrecht/refs/heads/main/authentication/utrecht-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Education
- Higher Education
- University
- Netherlands
- Research Data
- Open Access
- Library
- Open Source
---
