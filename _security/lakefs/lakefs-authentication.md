---
api_key_in:
- cookie
api_specs:
- filename: lakefs-openapi.yml
  format: yaml
  label: lakeFS
  slug: lakefs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/openapi/lakefs-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lakefs Authentication
name_suffix: Authentication
oauth_flows: []
overview: lakeFS secures its APIs with apiKey and http across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: lakeFS
provider_slug: lakefs
scheme_count: 5
schemes:
- name: basic_auth
  scheme: basic
  sources:
  - openapi/lakefs-openapi.yml
  type: http
- bearerFormat: JWT
  name: jwt_token
  scheme: bearer
  sources:
  - openapi/lakefs-openapi.yml
  type: http
- in: cookie
  name: cookie_auth
  parameter: internal_auth_session
  sources:
  - openapi/lakefs-openapi.yml
  type: apiKey
- in: cookie
  name: oidc_auth
  parameter: oidc_auth_session
  sources:
  - openapi/lakefs-openapi.yml
  type: apiKey
- in: cookie
  name: saml_auth
  parameter: saml_auth_session
  sources:
  - openapi/lakefs-openapi.yml
  type: apiKey
slug: lakefs-authentication
source_filename: lakefs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lakefs-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basic_auth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/lakefs-openapi.yml\n- name: jwt_token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/lakefs-openapi.yml\n- name: cookie_auth\n  type: apiKey\n  in: cookie\n  parameter: internal_auth_session\n  sources:\n  - openapi/lakefs-openapi.yml\n- name: oidc_auth\n  type: apiKey\n  in: cookie\n  parameter: oidc_auth_session\n  sources:\n  - openapi/lakefs-openapi.yml\n- name: saml_auth\n  type: apiKey\n  in: cookie\n  parameter: saml_auth_session\n  sources:\n  - openapi/lakefs-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lakefs/refs/heads/main/authentication/lakefs-authentication.yml
summary_line: apiKey/http · 5 schemes
tags:
- Data Version Control
- Data Lake
- Git-like
- Open Source
---
