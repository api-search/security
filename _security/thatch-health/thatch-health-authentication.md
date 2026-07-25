---
api_key_in:
- header
api_specs:
- filename: thatch-health-deductions-api-openapi.yml
  format: yaml
  label: Thatch Health Deductions API
  slug: thatch-health-deductions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/openapi/thatch-health-deductions-api-openapi.yml
- filename: thatch-health-employees-api-openapi.yml
  format: yaml
  label: Thatch Health Employees API
  slug: thatch-health-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/openapi/thatch-health-employees-api-openapi.yml
- filename: thatch-health-employer-onboarding-sessions-api-openapi.yml
  format: yaml
  label: Thatch Health Employer onboarding sessions API
  slug: thatch-health-employer-onboarding-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/openapi/thatch-health-employer-onboarding-sessions-api-openapi.yml
- filename: thatch-health-employers-api-openapi.yml
  format: yaml
  label: Thatch Health Employers API
  slug: thatch-health-employers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/openapi/thatch-health-employers-api-openapi.yml
- filename: thatch-health-enrollments-api-openapi.yml
  format: yaml
  label: Thatch Health Enrollments API
  slug: thatch-health-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/openapi/thatch-health-enrollments-api-openapi.yml
- filename: thatch-health-members-api-openapi.yml
  format: yaml
  label: Thatch Health Members API
  slug: thatch-health-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/openapi/thatch-health-members-api-openapi.yml
- filename: thatch-health-pay-schedules-api-openapi.yml
  format: yaml
  label: Thatch Health Pay Schedules API
  slug: thatch-health-pay-schedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/openapi/thatch-health-pay-schedules-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Thatch Health Authentication
name_suffix: Authentication
oauth_flows: []
overview: Thatch Health secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Thatch Health
provider_slug: thatch-health
scheme_count: 1
schemes:
- description: Provide your API key in a `Bearer` token header (as in, **Bearer sk_123**).
  in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/thatch-health-platforms-openapi-original.yml
  type: apiKey
slug: thatch-health-authentication
source_filename: thatch-health-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/thatch-health-platforms-openapi-original.yml\ndocs: https://docs.thatch.com/\nnotes: API keys are generated in the Thatch dashboard (app.thatch.com) and sent as\n  `Authorization Bearer <YOUR_API_KEY>` on every request; keys use an `sk_` prefix.\n  Partner accounts are provisioned by Thatch (platforms@thatch.com). Admin surfaces\n  on partners.thatchcloud.com and app.thatch.com expose OIDC discovery documents\n  (authorization-code flow, ES256), captured in well-known/.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Provide your API key in a `Bearer` token header (as in, **Bearer sk_123**).\n  sources:\n  - openapi/thatch-health-platforms-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/thatch-health/refs/heads/main/authentication/thatch-health-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Healthcare
- Health Benefits
- ICHRA
- Insurance
- Payroll
- Embedded Benefits
- HR
---
