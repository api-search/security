---
anonymous_access: false
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
- filename: workday-benefits-benefit-enrollment-event-offerings-openapi.json
  format: json
  label: Workday Benefit Enrollment Event Offerings API
  slug: workday-benefits-benefit-enrollment-event-offerings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-enrollment-event-offerings-openapi.json
- filename: workday-benefits-benefit-partner-openapi.json
  format: json
  label: Workday Benefit Partner API
  slug: workday-benefits-benefit-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/openapi/workday-benefits-benefit-partner-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Workday Benefits Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- implicit
overview: Workday Benefits secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and implicit flow(s).
provider_name: Workday Benefits
provider_slug: workday-benefits
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://<tenantAuthorizationHostname>
    flow: implicit
    scopes: 0
  name: OAuth2
  sources:
  - openapi/workday-benefits-benefit-enrollment-event-offerings-openapi.json
  - openapi/workday-benefits-benefit-partner-openapi.json
  type: oauth2
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token
  name: oauth2
  sources:
  - openapi/workday-benefits-benefit-enrollments-api-openapi.yml
  - openapi/workday-benefits-benefit-events-api-openapi.yml
  - openapi/workday-benefits-benefit-plans-api-openapi.yml
  - openapi/workday-benefits-dependents-api-openapi.yml
  - openapi/workday-benefits-employee-benefits-api-openapi.yml
  - openapi/workday-benefits-time-off-plans-api-openapi.yml
  type: oauth2
slug: workday-benefits-authentication
source_filename: workday-benefits-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: openapi/workday-benefits-benefit-enrollment-event-offerings-openapi.json, openapi/workday-benefits-benefit-enrollments-api-openapi.yml,\n  openapi/workday-benefits-benefit-events-api-openapi.yml, openapi/workday-benefits-benefit-partner-openapi.json,\n  openapi/workday-benefits-benefit-plans-api-openapi.yml, openapi/workday-benefits-dependents-api-openapi.yml, openapi/workday-benefits-employee-benefits-api-openapi.yml,\n  openapi/workday-benefits-time-off-plans-api-openapi.yml + https://developer.workday.com/doc/GUID-6c598444-ce67-40d5-bd95-267ecfe439b8-enHYPHENus.md\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  - implicit\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: implicit\n    authorizationUrl: https://<tenantAuthorizationHostname>\n    scopes: 0\n  sources:\n  - openapi/workday-benefits-benefit-enrollment-event-offerings-openapi.json\n  - openapi/workday-benefits-benefit-partner-openapi.json\n\
  - name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.workday.com/ccx/oauth2/{tenant}/token\n    scopes: 1\n  sources:\n  - openapi/workday-benefits-benefit-enrollments-api-openapi.yml\n  - openapi/workday-benefits-benefit-events-api-openapi.yml\n  - openapi/workday-benefits-benefit-plans-api-openapi.yml\n  - openapi/workday-benefits-dependents-api-openapi.yml\n  - openapi/workday-benefits-employee-benefits-api-openapi.yml\n  - openapi/workday-benefits-time-off-plans-api-openapi.yml\ndocs: https://developer.workday.com/doc/GUID-6c598444-ce67-40d5-bd95-267ecfe439b8-enHYPHENus.md\ndocumented:\n  model: OAuth 2.0 only - Workday requires OAuth to authenticate every REST API call.\n  client_registration: Register an API client on the Workday Developer Site / in the tenant (\"Register API Client\n    for Integrations\"), then choose an authorization flow to generate the access token.\n  flows_documented:\n  - authorization_code\n  - client_credentials\
  \ (server-to-server integrations)\n  - refresh_token\n  flow_in_contract: implicit - the two production Benefits contracts declare only components.securitySchemes.OAuth2\n    with an implicit flow and an unresolved https://<tenantAuthorizationHostname> authorization URL; Workday parameterises\n    the host per tenant rather than publishing a concrete authorization server.\n  token_endpoint: https://{tenantHostname}/ccx/oauth2/{tenant}/token\n  gateway: Extend and Orchestrate calls go through the regional API Gateway, which handles authentication and routes\n    to the tenant - https://developer.workday.com/doc/dlh1653340161856.md\n  authorization: A valid token is not sufficient. Workday enforces security domains on the integration system user;\n    a 403 \"Not Authorized\" means the domain has not been granted, and subresource access also requires permission\n    on the parent resource.\n  soap: The Benefits_Administration web service authenticates with WS-Security UsernameToken or OAuth\
  \ - https://developer.workday.com/doc/GUID-4c354bdb-06cd-461d-a632-ea8303beaedb-enHYPHENus.md\n  discovery: No /.well-known/openid-configuration or /.well-known/oauth-authorization-server document is served\n    on any Workday host probed 2026-09-17.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-benefits/refs/heads/main/authentication/workday-benefits-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Benefits
- Human Resources
- HCM
- Enterprise
- Payroll
- Employee Benefits
- SOAP
- OpenAPI
---
