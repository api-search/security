---
anonymous_access: false
api_key_in: []
api_specs:
- filename: klokin-io-accounting-api-openapi.yml
  format: yaml
  label: KLOKIN Accounting API
  slug: klokin-io-accounting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-accounting-api-openapi.yml
- filename: klokin-io-api-keys-api-openapi.yml
  format: yaml
  label: KLOKIN API keys API
  slug: klokin-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-api-keys-api-openapi.yml
- filename: klokin-io-audit-logs-api-openapi.yml
  format: yaml
  label: KLOKIN Audit logs API
  slug: klokin-io-audit-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-audit-logs-api-openapi.yml
- filename: klokin-io-auth-api-openapi.yml
  format: yaml
  label: KLOKIN Auth API
  slug: klokin-io-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-auth-api-openapi.yml
- filename: klokin-io-employees-api-openapi.yml
  format: yaml
  label: KLOKIN Employees API
  slug: klokin-io-employees-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-employees-api-openapi.yml
- filename: klokin-io-leave-api-openapi.yml
  format: yaml
  label: KLOKIN Leave API
  slug: klokin-io-leave-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-leave-api-openapi.yml
- filename: klokin-io-memberships-api-openapi.yml
  format: yaml
  label: KLOKIN Memberships API
  slug: klokin-io-memberships-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-memberships-api-openapi.yml
- filename: klokin-io-notifications-api-openapi.yml
  format: yaml
  label: KLOKIN Notifications API
  slug: klokin-io-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-notifications-api-openapi.yml
- filename: klokin-io-organizations-api-openapi.yml
  format: yaml
  label: KLOKIN Organizations API
  slug: klokin-io-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-organizations-api-openapi.yml
- filename: klokin-io-planning-api-openapi.yml
  format: yaml
  label: KLOKIN Planning API
  slug: klokin-io-planning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-planning-api-openapi.yml
- filename: klokin-io-reports-api-openapi.yml
  format: yaml
  label: KLOKIN Reports API
  slug: klokin-io-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-reports-api-openapi.yml
- filename: klokin-io-roles-api-openapi.yml
  format: yaml
  label: KLOKIN Roles API
  slug: klokin-io-roles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-roles-api-openapi.yml
- filename: klokin-io-schedules-api-openapi.yml
  format: yaml
  label: KLOKIN Schedules API
  slug: klokin-io-schedules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-schedules-api-openapi.yml
- filename: klokin-io-sso-api-openapi.yml
  format: yaml
  label: KLOKIN SSO API
  slug: klokin-io-sso-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-sso-api-openapi.yml
- filename: klokin-io-stores-api-openapi.yml
  format: yaml
  label: KLOKIN Stores API
  slug: klokin-io-stores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-stores-api-openapi.yml
- filename: klokin-io-system-api-openapi.yml
  format: yaml
  label: KLOKIN System API
  slug: klokin-io-system-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-system-api-openapi.yml
- filename: klokin-io-time-entries-api-openapi.yml
  format: yaml
  label: KLOKIN Time entries API
  slug: klokin-io-time-entries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-time-entries-api-openapi.yml
- filename: klokin-io-users-api-openapi.yml
  format: yaml
  label: KLOKIN Users API
  slug: klokin-io-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-users-api-openapi.yml
- filename: klokin-io-working-hours-api-openapi.yml
  format: yaml
  label: KLOKIN Working hours API
  slug: klokin-io-working-hours-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klokin-io/openapi/klokin-io-working-hours-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: KLOKIN Authentication
name_suffix: Authentication
oauth_flows: []
overview: KLOKIN secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: KLOKIN
provider_slug: klokin-io
scheme_count: 1
schemes:
- description: Admin JWT from POST /v1/auth/login, or a `klkn_…` API key.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/klokin-io-openapi.yml
  type: http
slug: klokin-io-authentication
source_filename: klokin-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/klokin-io-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Admin JWT from POST /v1/auth/login, or a `klkn_…` API key.\n  sources:\n  - openapi/klokin-io-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/klokin-io/authentication/klokin-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Time Tracking
- Payroll
- AI Assistant
- Lithuanian Law
- Software-as-a-Service
---
