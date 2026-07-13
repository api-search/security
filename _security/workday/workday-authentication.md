---
api_key_in: []
api_specs:
- filename: hcm.yml
  format: yaml
  label: Workday HCM API
  slug: hcm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/hcm.yml
- filename: financialManagement.yml
  format: yaml
  label: Workday Financial Management API
  slug: financial-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/financialManagement.yml
- filename: recruiting.yml
  format: yaml
  label: Workday Recruiting API
  slug: recruiting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/recruiting.yml
- filename: timeTracking.yml
  format: yaml
  label: Workday Time Tracking API
  slug: time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/timeTracking.yml
- filename: benefits.yml
  format: yaml
  label: Workday Benefits API
  slug: benefits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/benefits.yml
- filename: absenceManagement.yml
  format: yaml
  label: Workday Absence Management API
  slug: absence-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/absenceManagement.yml
- filename: compensation.yml
  format: yaml
  label: Workday Compensation API
  slug: compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/compensation.yml
- filename: payroll.yml
  format: yaml
  label: Workday Payroll API
  slug: payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/payroll.yml
- filename: person.yml
  format: yaml
  label: Workday Person API
  slug: person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/person.yml
- filename: performanceManagement.yml
  format: yaml
  label: Workday Performance Management API
  slug: performance-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/performanceManagement.yml
- filename: talent.yml
  format: yaml
  label: Workday Talent Management API
  slug: talent-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/talent.yml
- filename: common.yml
  format: yaml
  label: Workday Common API
  slug: common-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/common.yml
- filename: staffing.yml
  format: yaml
  label: Workday Staffing API
  slug: staffing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/staffing.yml
- filename: prismAnalytics.yml
  format: yaml
  label: Workday Prism Analytics API
  slug: prism-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/prismAnalytics.yml
- filename: raas.yml
  format: yaml
  label: Workday Report-as-a-Service API
  slug: raas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/raas.yml
- filename: wql.yml
  format: yaml
  label: Workday WQL API
  slug: wql-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/openapi/wql.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Workday secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Workday
provider_slug: workday
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token
  name: OAuth2
  sources:
  - openapi/absenceManagement.yml
  - openapi/benefits.yml
  - openapi/common.yml
  - openapi/compensation.yml
  - openapi/financialManagement.yml
  - openapi/hcm.yml
  - openapi/payroll.yml
  - openapi/performanceManagement.yml
  - openapi/person.yml
  - openapi/prismAnalytics.yml
  - openapi/raas.yml
  - openapi/recruiting.yml
  - openapi/staffing.yml
  - openapi/talent.yml
  - openapi/timeTracking.yml
  - openapi/wql.yml
  type: oauth2
- description: Basic authentication with Workday ISU credentials.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/raas.yml
  type: http
slug: workday-authentication
source_filename: workday-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/absenceManagement.yml, openapi/benefits.yml, openapi/common.yml, openapi/compensation.yml,\n  openapi/financialManagement.yml, openapi/hcm.yml, openapi/payroll.yml, openapi/performanceManagement.yml,\n  openapi/person.yml, openapi/prismAnalytics.yml, openapi/raas.yml, openapi/recruiting.yml ...\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/authorize\n    tokenUrl: https://wd2-impl-services1.workday.com/ccx/oauth2/{tenant}/token\n    scopes: 2\n  sources:\n  - openapi/absenceManagement.yml\n  - openapi/benefits.yml\n  - openapi/common.yml\n  - openapi/compensation.yml\n  - openapi/financialManagement.yml\n  - openapi/hcm.yml\n  - openapi/payroll.yml\n  - openapi/performanceManagement.yml\n  - openapi/person.yml\n  - openapi/prismAnalytics.yml\n\
  \  - openapi/raas.yml\n  - openapi/recruiting.yml\n  - openapi/staffing.yml\n  - openapi/talent.yml\n  - openapi/timeTracking.yml\n  - openapi/wql.yml\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: Basic authentication with Workday ISU credentials.\n  sources:\n  - openapi/raas.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday/refs/heads/main/authentication/workday-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Cloud Computing
- Enterprise Software
- Financial Management
- HCM
- SaaS
---
