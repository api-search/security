---
api_key_in: []
api_specs:
- filename: liferay-openapi.yml
  format: yaml
  label: Liferay Roles API
  slug: liferay
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/liferay/refs/heads/main/openapi/liferay-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Liferay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Liferay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Liferay
provider_slug: liferay
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/liferay-openapi.yml
  type: http
slug: liferay-authentication
source_filename: liferay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/liferay-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/liferay-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/liferay/refs/heads/main/authentication/liferay-authentication.yml
summary_line: http · 1 scheme
tags:
- Open Source
- Digital Experience
- DXP
- Roles
- Users
- Permissions
- Headless
---
