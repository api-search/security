---
api_key_in: []
api_specs:
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Companies API
  slug: nmbrs-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Employees API
  slug: nmbrs-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Employments API
  slug: nmbrs-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Payroll & Payruns API
  slug: nmbrs-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Wage Components API
  slug: nmbrs-wage-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Absences API
  slug: nmbrs-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
auth_types:
- oauth2
- apiKey
- soap-token
description: ''
kind: authentication
layout: security
method: documented
name: Nmbrs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nmbrs secures its APIs with oauth2, apiKey, and soap-token across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nmbrs
provider_slug: nmbrs
scheme_count: 3
schemes:
- authorizationUrl: https://identityservice.nmbrs.com/connect/authorize
  description: The current Nmbrs REST API uses the OAuth 2.0 Authorization Code flow. Authorization happens at the company/debtor level (not accountant login). Access is scoped with granular OAuth scopes.
  flow: authorizationCode
  name: oauth2
  scopes:
  - employee.info
  - employee.info.read
  - employee.employment
  - employee.employment.read
  - employee.payment
  sources:
  - https://developer.nmbrs.com/docs
  - https://nmbrs.stoplight.io/docs/nmbrs-restapi/ZG9jOjY4OTAxNTQ-authentication
  tokenUrl: https://identityservice.nmbrs.com/connect/token
  type: oauth2
- description: In addition to the OAuth bearer token, every REST request must carry a per-product subscription key generated when you subscribe to a product in the Nmbrs developer portal. Modeled here on an X-Subscription-Key header; confirm the exact header name in the Stoplight reference.
  in: header
  name: subscriptionKey
  sources:
  - https://developer.nmbrs.com/docs
  - https://nmbrs.stoplight.io/docs/nmbrs-restapi/ZG9jOjE5Nzc1OTky-getting-started
  type: apiKey
- description: The legacy SOAP v3 API authenticates with a username plus an API token passed in the SOAP AuthHeader. Deprecated; the SOAP API is scheduled to be retired on 1 March 2027.
  name: soapToken
  scheme: soap-header
  sources:
  - https://support.nmbrs.nl/hc/nl/articles/205903718-Nmbrs-API-for-developers
  - https://api.nmbrs.nl/soap/v3/EmployeeService.asmx
  type: apiKey
slug: nmbrs-authentication
source_filename: nmbrs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: documented\nsource: https://developer.nmbrs.com/docs\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  - soap-token\nschemes:\n- name: oauth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://identityservice.nmbrs.com/connect/authorize\n  tokenUrl: https://identityservice.nmbrs.com/connect/token\n  description: >-\n    The current Nmbrs REST API uses the OAuth 2.0 Authorization Code flow.\n    Authorization happens at the company/debtor level (not accountant login).\n    Access is scoped with granular OAuth scopes.\n  scopes:\n  - employee.info\n  - employee.info.read\n  - employee.employment\n  - employee.employment.read\n  - employee.payment\n  sources:\n  - https://developer.nmbrs.com/docs\n  - https://nmbrs.stoplight.io/docs/nmbrs-restapi/ZG9jOjY4OTAxNTQ-authentication\n- name: subscriptionKey\n  type: apiKey\n  in: header\n  description: >-\n    In addition to the OAuth bearer token, every REST request must carry a\n\
  \    per-product subscription key generated when you subscribe to a product in\n    the Nmbrs developer portal. Modeled here on an X-Subscription-Key header;\n    confirm the exact header name in the Stoplight reference.\n  sources:\n  - https://developer.nmbrs.com/docs\n  - https://nmbrs.stoplight.io/docs/nmbrs-restapi/ZG9jOjE5Nzc1OTky-getting-started\n- name: soapToken\n  type: apiKey\n  scheme: soap-header\n  description: >-\n    The legacy SOAP v3 API authenticates with a username plus an API token\n    passed in the SOAP AuthHeader. Deprecated; the SOAP API is scheduled to be\n    retired on 1 March 2027.\n  sources:\n  - https://support.nmbrs.nl/hc/nl/articles/205903718-Nmbrs-API-for-developers\n  - https://api.nmbrs.nl/soap/v3/EmployeeService.asmx\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/authentication/nmbrs-authentication.yml
summary_line: oauth2/apiKey/soap-token · 3 schemes
tags:
- Human Resources
- HRIS
- Payroll
- Employee Management
- HR
- Absence Management
- Netherlands
- Sweden
- SOAP
- REST
---
