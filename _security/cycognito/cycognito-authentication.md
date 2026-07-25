---
api_key_in:
- header
api_specs:
- filename: cycognito-assets-api-openapi.yml
  format: yaml
  label: CyCognito Assets API
  slug: cycognito-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-assets-api-openapi.yml
- filename: cycognito-audit-logs-api-openapi.yml
  format: yaml
  label: CyCognito Audit Logs API
  slug: cycognito-audit-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-audit-logs-api-openapi.yml
- filename: cycognito-cloud-connectors-api-openapi.yml
  format: yaml
  label: CyCognito Cloud Connectors API
  slug: cycognito-cloud-connectors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-cloud-connectors-api-openapi.yml
- filename: cycognito-export-data-api-openapi.yml
  format: yaml
  label: CyCognito Export Data API
  slug: cycognito-export-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-export-data-api-openapi.yml
- filename: cycognito-issues-api-openapi.yml
  format: yaml
  label: CyCognito Issues API
  slug: cycognito-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-issues-api-openapi.yml
- filename: cycognito-organizations-api-openapi.yml
  format: yaml
  label: CyCognito Organizations API
  slug: cycognito-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-organizations-api-openapi.yml
- filename: cycognito-realm-api-openapi.yml
  format: yaml
  label: CyCognito Realm API
  slug: cycognito-realm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-realm-api-openapi.yml
- filename: cycognito-reports-api-openapi.yml
  format: yaml
  label: CyCognito Reports API
  slug: cycognito-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-reports-api-openapi.yml
- filename: cycognito-revalidation-api-openapi.yml
  format: yaml
  label: CyCognito Revalidation API
  slug: cycognito-revalidation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-revalidation-api-openapi.yml
- filename: cycognito-scope-management-api-openapi.yml
  format: yaml
  label: CyCognito Scope Management API
  slug: cycognito-scope-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-scope-management-api-openapi.yml
- filename: cycognito-users-api-openapi.yml
  format: yaml
  label: CyCognito Users API
  slug: cycognito-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-users-api-openapi.yml
- filename: cycognito-verify-ips-api-openapi.yml
  format: yaml
  label: CyCognito Verify IPs API
  slug: cycognito-verify-ips-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/openapi/cycognito-verify-ips-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cycognito Authentication
name_suffix: Authentication
oauth_flows: []
overview: CyCognito secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CyCognito
provider_slug: cycognito
scheme_count: 1
schemes:
- in: header
  name: apiAuth
  parameter: Authorization
  sources:
  - openapi/cycognito-v1-openapi-original.json
  type: apiKey
slug: cycognito-authentication
source_filename: cycognito-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/cycognito-v1-openapi-original.json\ndocs: https://api.platform.cycognito.com/v1/docs/index.html\nnotes: API V1 authenticates with a user-generated API key in the Authorization header. Platform SSO is separately handled by an Auth0 tenant (auth.cycognito.com, OpenID Connect) and is not the API-key surface.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/cycognito-v1-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cycognito/refs/heads/main/authentication/cycognito-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Cybersecurity
- Attack Surface Management
- Exposure Management
- Security
- Vulnerability Management
- Cloud Security
- API Security
---
