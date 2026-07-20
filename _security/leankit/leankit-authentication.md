---
api_key_in: []
api_specs:
- filename: leankit-agileplace-api-openapi.yml
  format: yaml
  label: Planview AgilePlace API (LeanKit) v2
  slug: agileplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leankit/refs/heads/main/openapi/leankit-agileplace-api-openapi.yml
- filename: leankit-user-provisioning-api-openapi.yml
  format: yaml
  label: Planview AgilePlace User Provisioning API (SCIM 1.1)
  slug: user-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leankit/refs/heads/main/openapi/leankit-user-provisioning-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Leankit Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeanKit secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: LeanKit
provider_slug: leankit
scheme_count: 2
schemes:
- description: API token created via POST /io/auth/token or the "My API Tokens" tab in the AgilePlace user profile. Tokens do not expire; revoke unused tokens.
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/leankit-agileplace-api-openapi.yml
  - openapi/leankit-user-provisioning-api-openapi.yml
  type: http
- description: Base64-encoded AgilePlace email and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/leankit-agileplace-api-openapi.yml
  - openapi/leankit-user-provisioning-api-openapi.yml
  type: http
slug: leankit-authentication
source_filename: leankit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/leankit-agileplace-api-openapi.yml, openapi/leankit-user-provisioning-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  description: API token created via POST /io/auth/token or the \"My API Tokens\" tab in the AgilePlace\n    user profile. Tokens do not expire; revoke unused tokens.\n  sources:\n  - openapi/leankit-agileplace-api-openapi.yml\n  - openapi/leankit-user-provisioning-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Base64-encoded AgilePlace email and password.\n  sources:\n  - openapi/leankit-agileplace-api-openapi.yml\n  - openapi/leankit-user-provisioning-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leankit/refs/heads/main/authentication/leankit-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Kanban
- Project Management
- Agile
- Work Management
- Collaboration
- Enterprise Software
- Portfolio Management
- Workflow Automation
- SaaS
---
