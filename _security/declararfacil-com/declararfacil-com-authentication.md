---
anonymous_access: false
api_key_in: []
api_specs:
- filename: declararfacil-com-aeat-api-openapi.yml
  format: yaml
  label: Declarar Fácil Aeat API
  slug: declararfacil-com-aeat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-aeat-api-openapi.yml
- filename: declararfacil-com-agent-api-openapi.yml
  format: yaml
  label: Declarar Fácil Agent API
  slug: declararfacil-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-agent-api-openapi.yml
- filename: declararfacil-com-bank-expenses-api-openapi.yml
  format: yaml
  label: Declarar Fácil Bank Expenses API
  slug: declararfacil-com-bank-expenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-bank-expenses-api-openapi.yml
- filename: declararfacil-com-bank-income-api-openapi.yml
  format: yaml
  label: Declarar Fácil Bank Income API
  slug: declararfacil-com-bank-income-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-bank-income-api-openapi.yml
- filename: declararfacil-com-clients-api-openapi.yml
  format: yaml
  label: Declarar Fácil Clients API
  slug: declararfacil-com-clients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-clients-api-openapi.yml
- filename: declararfacil-com-dashboard-api-openapi.yml
  format: yaml
  label: Declarar Fácil Dashboard API
  slug: declararfacil-com-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-dashboard-api-openapi.yml
- filename: declararfacil-com-forms-api-openapi.yml
  format: yaml
  label: Declarar Fácil Forms API
  slug: declararfacil-com-forms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-forms-api-openapi.yml
- filename: declararfacil-com-historical-api-openapi.yml
  format: yaml
  label: Declarar Fácil Historical API
  slug: declararfacil-com-historical-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-historical-api-openapi.yml
- filename: declararfacil-com-invoices-api-openapi.yml
  format: yaml
  label: Declarar Fácil Invoices API
  slug: declararfacil-com-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-invoices-api-openapi.yml
- filename: declararfacil-com-manual-expenses-api-openapi.yml
  format: yaml
  label: Declarar Fácil Manual Expenses API
  slug: declararfacil-com-manual-expenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-manual-expenses-api-openapi.yml
- filename: declararfacil-com-tax-periods-api-openapi.yml
  format: yaml
  label: Declarar Fácil Tax Periods API
  slug: declararfacil-com-tax-periods-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-tax-periods-api-openapi.yml
- filename: declararfacil-com-user-api-openapi.yml
  format: yaml
  label: Declarar Fácil User API
  slug: declararfacil-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/declararfacil-com/openapi/declararfacil-com-user-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Declarar Fácil Authentication
name_suffix: Authentication
oauth_flows: []
overview: Declarar Fácil secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Declarar Fácil
provider_slug: declararfacil-com
scheme_count: 1
schemes:
- description: The df_ token handed out by the connect poll, or the last segment of the user's personal link (/agente/<token>).
  name: linkToken
  scheme: bearer
  sources:
  - openapi/declararfacil-com-agent-openapi.json
  - openapi/declararfacil-com-openapi.json
  type: http
slug: declararfacil-com-authentication
source_filename: declararfacil-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/declararfacil-com-agent-openapi.json, openapi/declararfacil-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: linkToken\n  type: http\n  scheme: bearer\n  description: The df_ token handed out by the connect poll, or the last segment of the user's\n    personal link (/agente/<token>).\n  sources:\n  - openapi/declararfacil-com-agent-openapi.json\n  - openapi/declararfacil-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/declararfacil-com/authentication/declararfacil-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Finance
- Accounting
- Tax
- Automation
- Artificial Intelligence
---
