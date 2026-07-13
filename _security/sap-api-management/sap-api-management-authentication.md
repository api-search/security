---
api_key_in: []
api_specs:
- filename: sap-api-management-portal-openapi.yml
  format: yaml
  label: SAP API Management API Portal API
  slug: sap-api-management-api-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-api-management/refs/heads/main/openapi/sap-api-management-portal-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Api Management Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP API Management secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP API Management
provider_slug: sap-api-management
scheme_count: 1
schemes:
- description: OAuth 2.0 authentication using SAP BTP service key credentials
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://{tenantUrl}/oauth/token
  name: OAuth2
  sources:
  - openapi/sap-api-management-portal-openapi.yml
  type: oauth2
slug: sap-api-management-authentication
source_filename: sap-api-management-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-api-management-portal-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenantUrl}/oauth/token\n    scopes: 1\n  description: OAuth 2.0 authentication using SAP BTP service key credentials\n  sources:\n  - openapi/sap-api-management-portal-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-api-management/refs/heads/main/authentication/sap-api-management-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- API Management
- Developer Portal
- Enterprise
- SAP
---
