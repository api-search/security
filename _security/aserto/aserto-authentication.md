---
api_key_in:
- header
api_specs:
- filename: aserto-decision-logs-api-openapi.yml
  format: yaml
  label: Aserto Decision Logs API
  slug: aserto-decision-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aserto/refs/heads/main/openapi/aserto-decision-logs-api-openapi.yml
- filename: aserto-authorizer-api-openapi.yml
  format: yaml
  label: Aserto Authorizer API
  slug: aserto-authorizer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aserto/refs/heads/main/openapi/aserto-authorizer-api-openapi.yml
- filename: aserto-authzen-api-openapi.yml
  format: yaml
  label: Aserto authzen API
  slug: aserto-authzen-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aserto/refs/heads/main/openapi/aserto-authzen-api-openapi.yml
- filename: aserto-decision-logs-api-openapi.yml
  format: yaml
  label: Aserto decision_logs API
  slug: aserto-decision-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aserto/refs/heads/main/openapi/aserto-decision-logs-api-openapi.yml
- filename: aserto-directory-api-openapi.yml
  format: yaml
  label: Aserto directory API
  slug: aserto-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aserto/refs/heads/main/openapi/aserto-directory-api-openapi.yml
- filename: aserto-info-api-openapi.yml
  format: yaml
  label: Aserto Info API
  slug: aserto-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aserto/refs/heads/main/openapi/aserto-info-api-openapi.yml
- filename: aserto-policy-api-openapi.yml
  format: yaml
  label: Aserto Policy API
  slug: aserto-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aserto/refs/heads/main/openapi/aserto-policy-api-openapi.yml
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
