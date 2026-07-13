---
api_key_in:
- header
api_specs:
- filename: stack-auth-openapi.yml
  format: yaml
  label: Stack Auth REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stack-auth/refs/heads/main/openapi/stack-auth-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Stack Auth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stack Auth secures its APIs with apiKey across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Stack Auth
provider_slug: stack-auth
scheme_count: 5
schemes:
- description: Project identifier for the Stack Auth project the request targets.
  in: header
  name: StackProjectId
  parameter: X-Stack-Project-Id
  sources:
  - openapi/stack-auth-openapi.yml
  type: apiKey
- description: One of "client", "server", or "admin".
  in: header
  name: StackAccessType
  parameter: X-Stack-Access-Type
  sources:
  - openapi/stack-auth-openapi.yml
  type: apiKey
- description: Publishable client key used for client access type.
  in: header
  name: StackPublishableClientKey
  parameter: X-Stack-Publishable-Client-Key
  sources:
  - openapi/stack-auth-openapi.yml
  type: apiKey
- description: Secret server key used for server access type.
  in: header
  name: StackSecretServerKey
  parameter: X-Stack-Secret-Server-Key
  sources:
  - openapi/stack-auth-openapi.yml
  type: apiKey
- description: Admin key used for admin access type.
  in: header
  name: StackSuperSecretAdminKey
  parameter: X-Stack-Super-Secret-Admin-Key
  sources:
  - openapi/stack-auth-openapi.yml
  type: apiKey
slug: stack-auth-authentication
source_filename: stack-auth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stack-auth-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: StackProjectId\n  type: apiKey\n  in: header\n  parameter: X-Stack-Project-Id\n  description: Project identifier for the Stack Auth project the request targets.\n  sources:\n  - openapi/stack-auth-openapi.yml\n- name: StackAccessType\n  type: apiKey\n  in: header\n  parameter: X-Stack-Access-Type\n  description: One of \"client\", \"server\", or \"admin\".\n  sources:\n  - openapi/stack-auth-openapi.yml\n- name: StackPublishableClientKey\n  type: apiKey\n  in: header\n  parameter: X-Stack-Publishable-Client-Key\n  description: Publishable client key used for client access type.\n  sources:\n  - openapi/stack-auth-openapi.yml\n- name: StackSecretServerKey\n  type: apiKey\n  in: header\n  parameter: X-Stack-Secret-Server-Key\n  description: Secret server key used for server access type.\n  sources:\n  - openapi/stack-auth-openapi.yml\n\
  - name: StackSuperSecretAdminKey\n  type: apiKey\n  in: header\n  parameter: X-Stack-Super-Secret-Admin-Key\n  description: Admin key used for admin access type.\n  sources:\n  - openapi/stack-auth-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stack-auth/refs/heads/main/authentication/stack-auth-authentication.yml
summary_line: apiKey · 5 schemes
tags:
- Authentication
- User Management
- Open Source
- Self-Hosted
- Identity
- Organizations
- RBAC
---
