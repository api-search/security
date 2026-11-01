---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: coderabbit-audit-logs-api-openapi.yml
  format: yaml
  label: CodeRabbit Audit Logs API
  slug: coderabbit-audit-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-audit-logs-api-openapi.yml
- filename: coderabbit-learnings-api-openapi.yml
  format: yaml
  label: CodeRabbit Learnings API
  slug: coderabbit-learnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-learnings-api-openapi.yml
- filename: coderabbit-metrics-api-openapi.yml
  format: yaml
  label: CodeRabbit Metrics API
  slug: coderabbit-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-metrics-api-openapi.yml
- filename: coderabbit-organizations-api-openapi.yml
  format: yaml
  label: CodeRabbit Organizations API
  slug: coderabbit-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-organizations-api-openapi.yml
- filename: coderabbit-report-generate-api-openapi.yml
  format: yaml
  label: CodeRabbit Report.generate API
  slug: coderabbit-report-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-report-generate-api-openapi.yml
- filename: coderabbit-role-management-api-openapi.yml
  format: yaml
  label: CodeRabbit Role Management API
  slug: coderabbit-role-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-role-management-api-openapi.yml
- filename: coderabbit-security-api-openapi.yml
  format: yaml
  label: CodeRabbit Security API
  slug: coderabbit-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-security-api-openapi.yml
- filename: coderabbit-users-api-openapi.yml
  format: yaml
  label: CodeRabbit Users API
  slug: coderabbit-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coderabbit/openapi/coderabbit-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Coderabbit Authentication
name_suffix: Authentication
oauth_flows: []
overview: CodeRabbit secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CodeRabbit
provider_slug: coderabbit
scheme_count: 1
schemes:
- description: CodeRabbit API key (format cr-xxxxxxxxxx), generated from the CodeRabbit organization settings and passed in the x-coderabbitai-api-key header.
  in: header
  name: apiKeyAuth
  parameter: x-coderabbitai-api-key
  sources:
  - openapi/coderabbit-openapi.yml
  type: apiKey
slug: coderabbit-authentication
source_filename: coderabbit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/coderabbit-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-coderabbitai-api-key\n  description: CodeRabbit API key (format cr-xxxxxxxxxx), generated from the CodeRabbit organization\n    settings and passed in the x-coderabbitai-api-key header.\n  sources:\n  - openapi/coderabbit-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/coderabbit/authentication/coderabbit-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Artificial Intelligence
- Code Review
- Developer Tools
- Pull Requests
- DevOps
---
