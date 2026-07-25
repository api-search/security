---
api_key_in: []
api_specs:
- filename: stackhawk-api-authentication-api-openapi.yml
  format: yaml
  label: StackHawk Api Authentication API
  slug: stackhawk-api-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-api-authentication-api-openapi.yml
- filename: stackhawk-applications-api-openapi.yml
  format: yaml
  label: StackHawk Applications API
  slug: stackhawk-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-applications-api-openapi.yml
- filename: stackhawk-global-configuration-api-openapi.yml
  format: yaml
  label: StackHawk Global Configuration API
  slug: stackhawk-global-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-global-configuration-api-openapi.yml
- filename: stackhawk-hosted-oas-api-openapi.yml
  format: yaml
  label: StackHawk Hosted OAS API
  slug: stackhawk-hosted-oas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-hosted-oas-api-openapi.yml
- filename: stackhawk-organization-teams-api-openapi.yml
  format: yaml
  label: StackHawk Organization Teams API
  slug: stackhawk-organization-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-organization-teams-api-openapi.yml
- filename: stackhawk-organizations-api-openapi.yml
  format: yaml
  label: StackHawk Organizations API
  slug: stackhawk-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-organizations-api-openapi.yml
- filename: stackhawk-perch-api-openapi.yml
  format: yaml
  label: StackHawk Perch API
  slug: stackhawk-perch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-perch-api-openapi.yml
- filename: stackhawk-profile-scans-api-openapi.yml
  format: yaml
  label: StackHawk Profile Scans API
  slug: stackhawk-profile-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-profile-scans-api-openapi.yml
- filename: stackhawk-reports-api-openapi.yml
  format: yaml
  label: StackHawk Reports API
  slug: stackhawk-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-reports-api-openapi.yml
- filename: stackhawk-repositories-api-openapi.yml
  format: yaml
  label: StackHawk Repositories API
  slug: stackhawk-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-repositories-api-openapi.yml
- filename: stackhawk-scan-configuration-api-openapi.yml
  format: yaml
  label: StackHawk Scan Configuration API
  slug: stackhawk-scan-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-scan-configuration-api-openapi.yml
- filename: stackhawk-scan-policies-api-openapi.yml
  format: yaml
  label: StackHawk Scan Policies API
  slug: stackhawk-scan-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-scan-policies-api-openapi.yml
- filename: stackhawk-scan-results-api-openapi.yml
  format: yaml
  label: StackHawk Scan Results API
  slug: stackhawk-scan-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-scan-results-api-openapi.yml
- filename: stackhawk-user-api-openapi.yml
  format: yaml
  label: StackHawk User API
  slug: stackhawk-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/openapi/stackhawk-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stackhawk Authentication
name_suffix: Authentication
oauth_flows: []
overview: StackHawk secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: StackHawk
provider_slug: stackhawk
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: JWT token obtained via /api/v1/auth/login
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/stackhawk-openapi.yml
  type: http
slug: stackhawk-authentication
source_filename: stackhawk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stackhawk-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained via /api/v1/auth/login\n  sources:\n  - openapi/stackhawk-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stackhawk/refs/heads/main/authentication/stackhawk-authentication.yml
summary_line: http · 1 scheme
tags:
- API Security
- Application Security
- DAST
- Security Testing
- Vulnerability Management
---
