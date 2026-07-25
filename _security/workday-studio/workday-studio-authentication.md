---
api_key_in: []
api_specs:
- filename: workday-studio-absence-management-api-openapi.yml
  format: yaml
  label: Workday Studio Absence Management API
  slug: workday-studio-absence-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-absence-management-api-openapi.yml
- filename: workday-studio-benefits-administration-api-openapi.yml
  format: yaml
  label: Workday Studio Benefits Administration API
  slug: workday-studio-benefits-administration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-benefits-administration-api-openapi.yml
- filename: workday-studio-compensation-api-openapi.yml
  format: yaml
  label: Workday Studio Compensation API
  slug: workday-studio-compensation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-compensation-api-openapi.yml
- filename: workday-studio-financial-management-api-openapi.yml
  format: yaml
  label: Workday Studio Financial Management API
  slug: workday-studio-financial-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-financial-management-api-openapi.yml
- filename: workday-studio-human-resources-api-openapi.yml
  format: yaml
  label: Workday Studio Human Resources API
  slug: workday-studio-human-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-human-resources-api-openapi.yml
- filename: workday-studio-integration-assemblies-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Assemblies API
  slug: workday-studio-integration-assemblies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-assemblies-api-openapi.yml
- filename: workday-studio-integration-events-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Events API
  slug: workday-studio-integration-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-events-api-openapi.yml
- filename: workday-studio-integration-systems-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Systems API
  slug: workday-studio-integration-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-systems-api-openapi.yml
- filename: workday-studio-integration-templates-api-openapi.yml
  format: yaml
  label: Workday Studio Integration Templates API
  slug: workday-studio-integration-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-integration-templates-api-openapi.yml
- filename: workday-studio-launch-parameters-api-openapi.yml
  format: yaml
  label: Workday Studio Launch Parameters API
  slug: workday-studio-launch-parameters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-launch-parameters-api-openapi.yml
- filename: workday-studio-payroll-api-openapi.yml
  format: yaml
  label: Workday Studio Payroll API
  slug: workday-studio-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-payroll-api-openapi.yml
- filename: workday-studio-recruiting-api-openapi.yml
  format: yaml
  label: Workday Studio Recruiting API
  slug: workday-studio-recruiting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-recruiting-api-openapi.yml
- filename: workday-studio-service-directory-api-openapi.yml
  format: yaml
  label: Workday Studio Service Directory API
  slug: workday-studio-service-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-service-directory-api-openapi.yml
- filename: workday-studio-staffing-api-openapi.yml
  format: yaml
  label: Workday Studio Staffing API
  slug: workday-studio-staffing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-staffing-api-openapi.yml
- filename: workday-studio-time-tracking-api-openapi.yml
  format: yaml
  label: Workday Studio Time Tracking API
  slug: workday-studio-time-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/openapi/workday-studio-time-tracking-api-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Workday Studio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Workday Studio secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Workday Studio
provider_slug: workday-studio
scheme_count: 2
schemes:
- flows:
  - authorizationUrl: https://{baseUrl}/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token
  name: OAuth2
  sources:
  - openapi/workday-studio-integration-openapi.yml
  - openapi/workday-studio-web-services-openapi.yml
  type: oauth2
- description: WS-Security with X.509 certificates or username/password tokens for SOAP API authentication.
  name: WSSecurity
  scheme: basic
  sources:
  - openapi/workday-studio-web-services-openapi.yml
  type: http
slug: workday-studio-authentication
source_filename: workday-studio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/workday-studio-integration-openapi.yml, openapi/workday-studio-web-services-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{baseUrl}/authorize\n    tokenUrl: https://{baseUrl}/oauth2/{tenant}/token\n    scopes: 2\n  sources:\n  - openapi/workday-studio-integration-openapi.yml\n  - openapi/workday-studio-web-services-openapi.yml\n- name: WSSecurity\n  type: http\n  scheme: basic\n  description: WS-Security with X.509 certificates or username/password tokens for SOAP API\n    authentication.\n  sources:\n  - openapi/workday-studio-web-services-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workday-studio/refs/heads/main/authentication/workday-studio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Cloud
- Development
- Enterprise
- Finance
- HR
- IDE
- Integration
---
