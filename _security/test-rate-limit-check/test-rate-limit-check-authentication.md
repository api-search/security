---
api_key_in:
- header
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Kong Gateway Admin API
  slug: kong-gateway-admin-api
  spec_type: OpenAPI
  url: https://docs.konghq.com/gateway/latest/admin-api/
- filename: x-tyk-gateway.json
  format: json
  label: Tyk API Management API
  slug: tyk-api-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/TykTechnologies/tyk/master/apidef/oas/schema/x-tyk-gateway.json
- filename: api-spec.json
  format: json
  label: Grafana API
  slug: grafana-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/grafana/grafana/main/public/api-spec.json
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
