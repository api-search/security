---
api_key_in:
- header
api_specs:
- filename: openapi-directory
  format: yaml
  label: Aserto Authorizer API
  slug: aserto-authorizer-api
  spec_type: OpenAPI
  url: https://github.com/aserto-dev/openapi-directory
- filename: openapi-directory
  format: yaml
  label: Aserto Directory API
  slug: aserto-directory-api
  spec_type: OpenAPI
  url: https://github.com/aserto-dev/openapi-directory
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aserto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Aserto secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Aserto
provider_slug: aserto
scheme_count: 2
schemes:
- in: header
  name: AuthorizerAPIKey
  parameter: authorization
  sources:
  - openapi/aserto-authorizer-openapi.yml
  - openapi/aserto-decision-logs-openapi.yml
  - openapi/aserto-directory-openapi.yml
  type: apiKey
- in: header
  name: TenantID
  parameter: aserto-tenant-id
  sources:
  - openapi/aserto-authorizer-openapi.yml
  - openapi/aserto-decision-logs-openapi.yml
  - openapi/aserto-directory-openapi.yml
  type: apiKey
slug: aserto-authentication
source_filename: aserto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/aserto-authorizer-openapi.yml, openapi/aserto-decision-logs-openapi.yml, openapi/aserto-directory-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AuthorizerAPIKey\n  type: apiKey\n  in: header\n  parameter: authorization\n  sources:\n  - openapi/aserto-authorizer-openapi.yml\n  - openapi/aserto-decision-logs-openapi.yml\n  - openapi/aserto-directory-openapi.yml\n- name: TenantID\n  type: apiKey\n  in: header\n  parameter: aserto-tenant-id\n  sources:\n  - openapi/aserto-authorizer-openapi.yml\n  - openapi/aserto-decision-logs-openapi.yml\n  - openapi/aserto-directory-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aserto/refs/heads/main/authentication/aserto-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Authorization
- Fine-Grained Access Control
- RBAC
- ABAC
- ReBAC
- Policy
- Open Policy Agent
- OPA
- Cloud-Native
- Security
---
