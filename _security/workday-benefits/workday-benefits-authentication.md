---
api_key_in: []
api_specs:
- filename: workday-benefits-benefit-enrollments-api-openapi.yml
  format: yaml
  label: Workday Benefits Benefit Enrollments API
  slug: workday-benefits-benefit-enrollments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-enrollments-api-openapi.yml
- filename: workday-benefits-benefit-events-api-openapi.yml
  format: yaml
  label: Workday Benefits Benefit Events API
  slug: workday-benefits-benefit-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-events-api-openapi.yml
- filename: workday-benefits-benefit-plans-api-openapi.yml
  format: yaml
  label: Workday Benefits Benefit Plans API
  slug: workday-benefits-benefit-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-plans-api-openapi.yml
- filename: workday-benefits-dependents-api-openapi.yml
  format: yaml
  label: Workday Benefits Dependents API
  slug: workday-benefits-dependents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-dependents-api-openapi.yml
- filename: workday-benefits-employee-benefits-api-openapi.yml
  format: yaml
  label: Workday Benefits Employee Benefits API
  slug: workday-benefits-employee-benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-employee-benefits-api-openapi.yml
- filename: workday-benefits-time-off-plans-api-openapi.yml
  format: yaml
  label: Workday Benefits Time Off Plans API
  slug: workday-benefits-time-off-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-time-off-plans-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Benefits Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Workday Benefits secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Workday Benefits
provider_slug: workday-benefits
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  sources:
  - openapi/workday-benefits-openapi.yml
  type: oauth2
slug: workday-benefits-authentication
source_filename: workday-benefits-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-benefits-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n    scopes: 1\n  sources:\n  - openapi/workday-benefits-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/authentication/workday-benefits-authentication.yml
summary_line: oauth2 · 1 scheme
tags: []
---
