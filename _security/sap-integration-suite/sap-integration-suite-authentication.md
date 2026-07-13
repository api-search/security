---
api_key_in: []
api_specs:
- filename: sap-integration-suite-cloud-integration-openapi.yml
  format: yaml
  label: SAP Cloud Integration API
  slug: sap-cloud-integration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-cloud-integration-openapi.yml
- filename: sap-integration-suite-api-management-openapi.yml
  format: yaml
  label: SAP API Management API
  slug: sap-api-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/openapi/sap-integration-suite-api-management-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Integration Suite Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP Integration Suite secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP Integration Suite
provider_slug: sap-integration-suite
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token
  name: oauth2
  sources:
  - openapi/sap-integration-suite-api-management-openapi.yml
  - openapi/sap-integration-suite-cloud-integration-openapi.yml
  type: oauth2
- name: basicAuth
  scheme: basic
  sources:
  - openapi/sap-integration-suite-api-management-openapi.yml
  type: http
slug: sap-integration-suite-authentication
source_filename: sap-integration-suite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-integration-suite-api-management-openapi.yml, openapi/sap-integration-suite-cloud-integration-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.authentication.sap.hana.ondemand.com/oauth/token\n    scopes: 0\n  sources:\n  - openapi/sap-integration-suite-api-management-openapi.yml\n  - openapi/sap-integration-suite-cloud-integration-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/sap-integration-suite-api-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-integration-suite/refs/heads/main/authentication/sap-integration-suite-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- API Management
- Cloud Integration
- Enterprise Integration
- Event Mesh
- iPaaS
- SAP
- SAP BTP
---
