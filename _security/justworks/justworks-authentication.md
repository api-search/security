---
api_key_in: []
api_specs:
- filename: justworks-members-api-openapi.yml
  format: yaml
  label: Justworks Members API
  slug: justworks-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-members-api-openapi.yml
- filename: justworks-company-api-openapi.yml
  format: yaml
  label: Justworks Company API
  slug: justworks-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-company-api-openapi.yml
- filename: justworks-deductions-api-openapi.yml
  format: yaml
  label: Justworks Deductions API
  slug: justworks-deductions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-deductions-api-openapi.yml
- filename: justworks-webhooks-api-openapi.yml
  format: yaml
  label: Justworks Webhooks API
  slug: justworks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-webhooks-api-openapi.yml
- filename: justworks-oauth-api-openapi.yml
  format: yaml
  label: Justworks OAuth API
  slug: justworks-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-oauth-api-openapi.yml
- filename: justworks-deduction-types-api-openapi.yml
  format: yaml
  label: Justworks Deduction Types API
  slug: justworks-deduction-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-deduction-types-api-openapi.yml
- filename: justworks-payrolls-api-openapi.yml
  format: yaml
  label: Justworks Payrolls API
  slug: justworks-payrolls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-payrolls-api-openapi.yml
- filename: justworks-paystubs-api-openapi.yml
  format: yaml
  label: Justworks Paystubs API
  slug: justworks-paystubs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-paystubs-api-openapi.yml
- filename: justworks-time-off-balances-api-openapi.yml
  format: yaml
  label: Justworks Time Off Balances API
  slug: justworks-time-off-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-time-off-balances-api-openapi.yml
- filename: justworks-time-off-policies-api-openapi.yml
  format: yaml
  label: Justworks Time Off Policies API
  slug: justworks-time-off-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-time-off-policies-api-openapi.yml
- filename: justworks-time-off-requests-api-openapi.yml
  format: yaml
  label: Justworks Time Off Requests API
  slug: justworks-time-off-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/openapi/justworks-time-off-requests-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Justworks Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Justworks secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Justworks
provider_slug: justworks
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://secure.justworks.com/oauth/authorize
    flow: authorizationCode
    scopes: 3
    tokenUrl: https://public-api.justworks.com/oauth/token
  name: OAuth2
  sources:
  - openapi/justworks-company-api-openapi.yml
  - openapi/justworks-deductions-api-openapi.yml
  - openapi/justworks-members-api-openapi.yml
  - openapi/justworks-payroll-api-openapi.yml
  - openapi/justworks-time-off-api-openapi.yml
  - openapi/justworks-webhooks-api-openapi.yml
  type: oauth2
slug: justworks-authentication
source_filename: justworks-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/justworks-company-api-openapi.yml, openapi/justworks-deductions-api-openapi.yml,\n  openapi/justworks-members-api-openapi.yml, openapi/justworks-payroll-api-openapi.yml, openapi/justworks-time-off-api-openapi.yml,\n  openapi/justworks-webhooks-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://secure.justworks.com/oauth/authorize\n    tokenUrl: https://public-api.justworks.com/oauth/token\n    scopes: 3\n  sources:\n  - openapi/justworks-company-api-openapi.yml\n  - openapi/justworks-deductions-api-openapi.yml\n  - openapi/justworks-members-api-openapi.yml\n  - openapi/justworks-payroll-api-openapi.yml\n  - openapi/justworks-time-off-api-openapi.yml\n  - openapi/justworks-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justworks/refs/heads/main/authentication/justworks-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- PEO
- Payroll
- HR
- Human Resources
- Benefits
- Health Insurance
- 401(k)
- Time Off
- Compliance
- Small Business
- Employer of Record
- HRIS
---
