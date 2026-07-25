---
api_key_in: []
api_specs:
- filename: keka-assets-api-openapi.yml
  format: yaml
  label: Keka HR Assets API
  slug: keka-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-assets-api-openapi.yml
- filename: keka-attendance-api-openapi.yml
  format: yaml
  label: Keka HR Attendance API
  slug: keka-attendance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-attendance-api-openapi.yml
- filename: keka-authentication-api-openapi.yml
  format: yaml
  label: Keka HR Authentication API
  slug: keka-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-authentication-api-openapi.yml
- filename: keka-bgv-apis-api-openapi.yml
  format: yaml
  label: Keka HR BGV APIs API
  slug: keka-bgv-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-bgv-apis-api-openapi.yml
- filename: keka-core-hr-api-openapi.yml
  format: yaml
  label: Keka HR Core HR API
  slug: keka-core-hr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-core-hr-api-openapi.yml
- filename: keka-documents-api-openapi.yml
  format: yaml
  label: Keka HR Documents API
  slug: keka-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-documents-api-openapi.yml
- filename: keka-expense-api-openapi.yml
  format: yaml
  label: Keka HR Expense API
  slug: keka-expense-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-expense-api-openapi.yml
- filename: keka-hire-api-openapi.yml
  format: yaml
  label: Keka HR Hire API
  slug: keka-hire-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-hire-api-openapi.yml
- filename: keka-leave-api-openapi.yml
  format: yaml
  label: Keka HR Leave API
  slug: keka-leave-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-leave-api-openapi.yml
- filename: keka-payroll-api-openapi.yml
  format: yaml
  label: Keka HR Payroll API
  slug: keka-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-payroll-api-openapi.yml
- filename: keka-pms-api-openapi.yml
  format: yaml
  label: Keka HR PMS API
  slug: keka-pms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-pms-api-openapi.yml
- filename: keka-psa-api-openapi.yml
  format: yaml
  label: Keka HR PSA API
  slug: keka-psa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-psa-api-openapi.yml
- filename: keka-requisitions-api-openapi.yml
  format: yaml
  label: Keka HR Requisitions API
  slug: keka-requisitions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-requisitions-api-openapi.yml
- filename: keka-skills-api-openapi.yml
  format: yaml
  label: Keka HR Skills API
  slug: keka-skills-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/openapi/keka-skills-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Keka Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Keka HR secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Keka HR
provider_slug: keka
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials flow
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://login.keka.com/connect/token
  name: oauth2
  sources:
  - openapi/keka-hr-api-openapi.yaml
  type: oauth2
slug: keka-authentication
source_filename: keka-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/keka-hr-api-openapi.yaml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://login.keka.com/connect/token\n    scopes: 1\n  description: OAuth 2.0 client credentials flow\n  sources:\n  - openapi/keka-hr-api-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keka/refs/heads/main/authentication/keka-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- HR
- Human Resources
- Payroll
- Attendance
- Leave Management
- Performance Management
- Employee Management
- India
- HRMS
---
