---
api_key_in: []
api_specs:
- filename: humaans-io-audit-events-api-openapi.yml
  format: yaml
  label: Humaans Audit Events API
  slug: humaans-io-audit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-audit-events-api-openapi.yml
- filename: humaans-io-bank-accounts-api-openapi.yml
  format: yaml
  label: Humaans Bank Accounts API
  slug: humaans-io-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-bank-accounts-api-openapi.yml
- filename: humaans-io-companies-api-openapi.yml
  format: yaml
  label: Humaans Companies API
  slug: humaans-io-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-companies-api-openapi.yml
- filename: humaans-io-compensations-api-openapi.yml
  format: yaml
  label: Humaans Compensations API
  slug: humaans-io-compensations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-compensations-api-openapi.yml
- filename: humaans-io-custom-fields-api-openapi.yml
  format: yaml
  label: Humaans Custom Fields API
  slug: humaans-io-custom-fields-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-custom-fields-api-openapi.yml
- filename: humaans-io-documents-api-openapi.yml
  format: yaml
  label: Humaans Documents API
  slug: humaans-io-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-documents-api-openapi.yml
- filename: humaans-io-equipment-api-openapi.yml
  format: yaml
  label: Humaans Equipment API
  slug: humaans-io-equipment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-equipment-api-openapi.yml
- filename: humaans-io-job-roles-api-openapi.yml
  format: yaml
  label: Humaans Job Roles API
  slug: humaans-io-job-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-job-roles-api-openapi.yml
- filename: humaans-io-locations-api-openapi.yml
  format: yaml
  label: Humaans Locations API
  slug: humaans-io-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-locations-api-openapi.yml
- filename: humaans-io-people-api-openapi.yml
  format: yaml
  label: Humaans People API
  slug: humaans-io-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-people-api-openapi.yml
- filename: humaans-io-performance-api-openapi.yml
  format: yaml
  label: Humaans Performance API
  slug: humaans-io-performance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-performance-api-openapi.yml
- filename: humaans-io-time-away-api-openapi.yml
  format: yaml
  label: Humaans Time Away API
  slug: humaans-io-time-away-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-time-away-api-openapi.yml
- filename: humaans-io-timesheet-api-openapi.yml
  format: yaml
  label: Humaans Timesheet API
  slug: humaans-io-timesheet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-timesheet-api-openapi.yml
- filename: humaans-io-webhooks-api-openapi.yml
  format: yaml
  label: Humaans Webhooks API
  slug: humaans-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-webhooks-api-openapi.yml
- filename: humaans-io-working-patterns-api-openapi.yml
  format: yaml
  label: Humaans Working Patterns API
  slug: humaans-io-working-patterns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/openapi/humaans-io-working-patterns-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Humaans Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Humaans secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Humaans
provider_slug: humaans-io
scheme_count: 1
schemes:
- bearerFormat: token
  description: Bearer access token issued by Humaans with OAuth-style scopes
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/humaans-api-openapi.yml
  type: http
slug: humaans-io-authentication
source_filename: humaans-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/humaans-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  description: Bearer access token issued by Humaans with OAuth-style scopes\n  sources:\n  - openapi/humaans-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humaans-io/refs/heads/main/authentication/humaans-io-authentication.yml
summary_line: http · 1 scheme
tags:
- HR
- HRIS
- Human Resources
- People Operations
- People Analytics
- Onboarding
- Offboarding
- Performance Management
- Time Off
- Compensation
- Workflow-Automation
- AI Companion
- Agentic AI
- UK
- London
---
