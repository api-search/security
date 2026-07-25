---
api_key_in:
- header
api_specs:
- filename: test-rate-limit-check-consumers-api-openapi.yml
  format: yaml
  label: Test Rate Limit Check Consumers API
  slug: test-rate-limit-check-consumers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/test-rate-limit-check/refs/heads/main/openapi/test-rate-limit-check-consumers-api-openapi.yml
- filename: test-rate-limit-check-plugins-api-openapi.yml
  format: yaml
  label: Test Rate Limit Check Plugins API
  slug: test-rate-limit-check-plugins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/test-rate-limit-check/refs/heads/main/openapi/test-rate-limit-check-plugins-api-openapi.yml
- filename: test-rate-limit-check-routes-api-openapi.yml
  format: yaml
  label: Test Rate Limit Check Routes API
  slug: test-rate-limit-check-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/test-rate-limit-check/refs/heads/main/openapi/test-rate-limit-check-routes-api-openapi.yml
- filename: test-rate-limit-check-schemas-api-openapi.yml
  format: yaml
  label: Test Rate Limit Check Schemas API
  slug: test-rate-limit-check-schemas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/test-rate-limit-check/refs/heads/main/openapi/test-rate-limit-check-schemas-api-openapi.yml
- filename: test-rate-limit-check-services-api-openapi.yml
  format: yaml
  label: Test Rate Limit Check Services API
  slug: test-rate-limit-check-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/test-rate-limit-check/refs/heads/main/openapi/test-rate-limit-check-services-api-openapi.yml
- filename: test-rate-limit-check-status-api-openapi.yml
  format: yaml
  label: Test Rate Limit Check Status API
  slug: test-rate-limit-check-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/test-rate-limit-check/refs/heads/main/openapi/test-rate-limit-check-status-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Test Rate Limit Check Authentication
name_suffix: Authentication
oauth_flows: []
overview: Test Rate Limit Check secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Test Rate Limit Check
provider_slug: test-rate-limit-check
scheme_count: 1
schemes:
- description: RBAC admin token issued by Kong Gateway when RBAC is enabled.
  in: header
  name: rbacToken
  parameter: Kong-Admin-Token
  sources:
  - openapi/test-rate-limit-check-openapi.yml
  type: apiKey
slug: test-rate-limit-check-authentication
source_filename: test-rate-limit-check-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/test-rate-limit-check-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: rbacToken\n  type: apiKey\n  in: header\n  parameter: Kong-Admin-Token\n  description: RBAC admin token issued by Kong Gateway when RBAC is enabled.\n  sources:\n  - openapi/test-rate-limit-check-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/test-rate-limit-check/refs/heads/main/authentication/test-rate-limit-check-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Governance
- API Management
- API Testing
- Performance Testing
- Rate Limiting
- Testing
---
