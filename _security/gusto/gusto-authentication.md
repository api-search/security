---
api_key_in: []
api_specs:
- filename: gusto-asyncapi.yml
  format: yaml
  label: Gusto Embedded Payroll API
  slug: embedded-payroll-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-asyncapi.yml
- filename: gusto-bankaccounts-api-openapi.yml
  format: yaml
  label: Gusto BankAccounts API
  slug: gusto-bankaccounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-bankaccounts-api-openapi.yml
- filename: gusto-companies-api-openapi.yml
  format: yaml
  label: Gusto Companies API
  slug: gusto-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-companies-api-openapi.yml
- filename: gusto-contractorpayments-api-openapi.yml
  format: yaml
  label: Gusto ContractorPayments API
  slug: gusto-contractorpayments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-contractorpayments-api-openapi.yml
- filename: gusto-contractors-api-openapi.yml
  format: yaml
  label: Gusto Contractors API
  slug: gusto-contractors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-contractors-api-openapi.yml
- filename: gusto-employees-api-openapi.yml
  format: yaml
  label: Gusto Employees API
  slug: gusto-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-employees-api-openapi.yml
- filename: gusto-flows-api-openapi.yml
  format: yaml
  label: Gusto Flows API
  slug: gusto-flows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-flows-api-openapi.yml
- filename: gusto-payrolls-api-openapi.yml
  format: yaml
  label: Gusto Payrolls API
  slug: gusto-payrolls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-payrolls-api-openapi.yml
- filename: gusto-payschedules-api-openapi.yml
  format: yaml
  label: Gusto PaySchedules API
  slug: gusto-payschedules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-payschedules-api-openapi.yml
- filename: gusto-reports-api-openapi.yml
  format: yaml
  label: Gusto Reports API
  slug: gusto-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-reports-api-openapi.yml
- filename: gusto-webhooks-api-openapi.yml
  format: yaml
  label: Gusto Webhooks API
  slug: gusto-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/openapi/gusto-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gusto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gusto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Gusto
provider_slug: gusto
scheme_count: 1
schemes:
- description: 'OAuth 2.0 access token for company-level access or system-level bearer

    token for partner operations. Scopes such as payrolls:read, payrolls:run,

    contractors:write provide fine-grained permissions.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/gusto-openapi.yml
  type: http
slug: gusto-authentication
source_filename: gusto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gusto-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    OAuth 2.0 access token for company-level access or system-level bearer\n    token for partner operations. Scopes such as payrolls:read, payrolls:run,\n    contractors:write provide fine-grained permissions.\n  sources:\n  - openapi/gusto-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gusto/refs/heads/main/authentication/gusto-authentication.yml
summary_line: http · 1 scheme
tags:
- Human Resources
- Payroll
- Benefits
- Enterprise Software
- Embedded Finance
---
