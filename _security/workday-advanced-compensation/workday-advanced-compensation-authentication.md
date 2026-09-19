---
anonymous_access: false
api_key_in: []
api_specs:
- filename: workday-advanced-compensation-compensation-rest-v3-openapi.json
  format: json
  label: Workday Compensation REST API v3
  slug: workday-compensation-rest-v3
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/workday-advanced-compensation-compensation-rest-v3-openapi.json
- filename: workday-advanced-compensation-bonus-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Bonus Plans API
  slug: workday-advanced-compensation-bonus-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-bonus-plans-api-openapi.yml
- filename: workday-advanced-compensation-compensation-budgets-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Budgets API
  slug: workday-advanced-compensation-compensation-budgets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-budgets-api-openapi.yml
- filename: workday-advanced-compensation-compensation-grades-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Grades API
  slug: workday-advanced-compensation-compensation-grades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-grades-api-openapi.yml
- filename: workday-advanced-compensation-compensation-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Plans API
  slug: workday-advanced-compensation-compensation-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-plans-api-openapi.yml
- filename: workday-advanced-compensation-compensation-reviews-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Reviews API
  slug: workday-advanced-compensation-compensation-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-compensation-reviews-api-openapi.yml
- filename: workday-advanced-compensation-employee-compensation-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Employee Compensation API
  slug: workday-advanced-compensation-employee-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-employee-compensation-api-openapi.yml
- filename: workday-advanced-compensation-merit-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Merit Plans API
  slug: workday-advanced-compensation-merit-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-merit-plans-api-openapi.yml
- filename: workday-advanced-compensation-stock-plans-api-openapi.yml
  format: yaml
  label: Workday Advanced Compensation Stock Plans API
  slug: workday-advanced-compensation-stock-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/openapi/_ae-authored/workday-advanced-compensation-stock-plans-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Workday Advanced Compensation Authentication
name_suffix: Authentication
oauth_flows:
- implicit
- authorizationCode
- clientCredentials
overview: Workday Advanced Compensation secures its APIs with oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit, authorizationCode, and clientCredentials flow(s).
provider_name: Workday Advanced Compensation
provider_slug: workday-advanced-compensation
scheme_count: 4
schemes:
- description: Declared verbatim in Workday's published compensation v1/v2/v3 OpenAPI documents. The authorization host is tenant-specific and is left templated by Workday.
  flows:
  - authorizationUrl: https://<tenantAuthorizationHostname>
    flow: implicit
    scopes: 0
  name: OAuth2
  sources:
  - openapi/_original/workday-advanced-compensation-compensation-v3-openapi.json
  - openapi/_original/workday-advanced-compensation-compensation-v2-openapi.json
  - openapi/_original/workday-advanced-compensation-compensation-v1-openapi.json
  type: oauth2
- description: Documented grant for apps acting in a signed-in Workday user's context.
  flows:
  - flow: authorizationCode
  name: OAuth2 Authorization Code
  sources:
  - https://developer.workday.com/doc/jzx1537909761291.md
  type: oauth2
- description: 'Documented grant for server-to-server integrations. The API Client is registered in the tenant and bound to an Integration System User whose security groups carry the domains the operations name (e.g. "Set Up: Merit and Bonus").'
  flows:
  - flow: clientCredentials
  name: OAuth2 Client Credentials (Integration System User)
  sources:
  - https://developer.workday.com/doc/axp1537909839739.md
  type: oauth2
- description: Workday Web Services (SOAP) authentication for the Compensation and Compensation_Review WSDLs, using an Integration System User account scoped to the tenant.
  name: WS-Security UsernameToken
  scheme: ws-security
  sources:
  - wsdl/workday-advanced-compensation-compensation.wsdl
  type: http
slug: workday-advanced-compensation-authentication
source_filename: workday-advanced-compensation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/_original/workday-advanced-compensation-compensation-v3-openapi.json\ndocs: https://developer.workday.com/doc/axp1537909839739.md\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - implicit\n  - authorizationCode\n  - clientCredentials\n  api_key_in: []\n  note: >-\n    OAuth 2.0 only. Workday's published compensation OpenAPI declares a single OAuth2 scheme with\n    the implicit flow against a templated tenant authorization host; the developer documentation\n    documents Authorization Code (user-context apps) and Client Credentials with an Integration\n    System User (server-to-server) as the supported grants. The SOAP Workday Web Services surface\n    additionally accepts WS-Security UsernameToken with an ISU account.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://<tenantAuthorizationHostname>\n    scopes: 0\n  description: >-\n    Declared verbatim in Workday's\
  \ published compensation v1/v2/v3 OpenAPI documents. The\n    authorization host is tenant-specific and is left templated by Workday.\n  sources:\n  - openapi/_original/workday-advanced-compensation-compensation-v3-openapi.json\n  - openapi/_original/workday-advanced-compensation-compensation-v2-openapi.json\n  - openapi/_original/workday-advanced-compensation-compensation-v1-openapi.json\n- name: OAuth2 Authorization Code\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n  description: Documented grant for apps acting in a signed-in Workday user's context.\n  sources:\n  - https://developer.workday.com/doc/jzx1537909761291.md\n- name: OAuth2 Client Credentials (Integration System User)\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n  description: >-\n    Documented grant for server-to-server integrations. The API Client is registered in the\n    tenant and bound to an Integration System User whose security groups carry the domains the\n    operations name (e.g. \"Set Up:\
  \ Merit and Bonus\").\n  sources:\n  - https://developer.workday.com/doc/axp1537909839739.md\n- name: WS-Security UsernameToken\n  type: http\n  scheme: ws-security\n  description: >-\n    Workday Web Services (SOAP) authentication for the Compensation and Compensation_Review\n    WSDLs, using an Integration System User account scoped to the tenant.\n  sources:\n  - wsdl/workday-advanced-compensation-compensation.wsdl\ngateways:\n  note: >-\n    Workday Extend / Workday Cloud Platform API gateway and authorization base URLs are\n    region-specific and published by Workday.\n  source: https://developer.workday.com/doc/dlh1653340161856.md\n  regions:\n  - region: United States\n    api_gateway: https://api.workday.com\n    authorization_base_url: https://auth.api.workday.com\n  - region: Germany\n    api_gateway: https://api.eu.wcp.workday.com\n    authorization_base_url: https://api.eu.wcp.workday.com/auth\n  - region: Singapore\n    api_gateway: https://api.sg.wcp.workday.com\n    authorization_base_url:\
  \ https://api.sg.wcp.workday.com/auth\n  - region: United Kingdom\n    api_gateway: https://api.uk.wcp.workday.com\n    authorization_base_url: https://api.uk.wcp.workday.com/auth\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-advanced-compensation/refs/heads/main/authentication/workday-advanced-compensation-authentication.yml
summary_line: oauth2 · 4 schemes
tags:
- Compensation
- Human Resources
- Payroll
- HCM
- Enterprise Software
- Total Rewards
- Bonus
- Merit
- Stock Compensation
- SOAP
- Software-as-a-Service
---
