---
api_key_in: []
api_specs:
- filename: sap-fieldglass-approval-openapi.yaml
  format: yaml
  label: SAP Fieldglass Approval API
  slug: sap-fieldglass-approval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-approval-openapi.yaml
- filename: sap-fieldglass-odata-analytic-openapi.json
  format: json
  label: SAP Fieldglass OData-Based Analytic API
  slug: sap-fieldglass-odata-based-analytic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-odata-analytic-openapi.json
- filename: sap-fieldglass-background-check-openapi.json
  format: json
  label: SAP Fieldglass Background Check API
  slug: sap-fieldglass-background-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-background-check-openapi.json
- filename: sap-fieldglass-audit-trail-openapi.json
  format: json
  label: SAP Fieldglass Audit Trail API
  slug: sap-fieldglass-audit-trail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-audit-trail-openapi.json
- filename: sap-fieldglass-business-analytics-openapi.json
  format: json
  label: SAP Fieldglass Business Analytics API
  slug: sap-fieldglass-business-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/openapi/sap-fieldglass-business-analytics-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Fieldglass Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP Fieldglass secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP Fieldglass
provider_slug: sap-fieldglass
scheme_count: 1
schemes:
- description: To use this REST API, you need to get OAuth client credentials (user credentials and client-specific application key) from an SAP Fieldglass account representative. After that, you need to pass the obtained client credentials to the SAP Fieldglass token endpoint to obtain an access token.
  flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: ' '
  name: OAuth2
  sources:
  - openapi/sap-fieldglass-approval-openapi.yaml
  - openapi/sap-fieldglass-audit-trail-openapi.json
  - openapi/sap-fieldglass-background-check-openapi.json
  - openapi/sap-fieldglass-business-analytics-openapi.json
  - openapi/sap-fieldglass-odata-analytic-openapi.json
  type: oauth2
slug: sap-fieldglass-authentication
source_filename: sap-fieldglass-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-fieldglass-approval-openapi.yaml, openapi/sap-fieldglass-audit-trail-openapi.json,\n  openapi/sap-fieldglass-background-check-openapi.json, openapi/sap-fieldglass-business-analytics-openapi.json,\n  openapi/sap-fieldglass-odata-analytic-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: ' '\n    scopes: 1\n  description: To use this REST API, you need to get OAuth client credentials (user credentials\n    and client-specific application key) from an SAP Fieldglass account representative. After\n    that, you need to pass the obtained client credentials to the SAP Fieldglass token endpoint\n    to obtain an access token.\n  sources:\n  - openapi/sap-fieldglass-approval-openapi.yaml\n  - openapi/sap-fieldglass-audit-trail-openapi.json\n  - openapi/sap-fieldglass-background-check-openapi.json\n\
  \  - openapi/sap-fieldglass-business-analytics-openapi.json\n  - openapi/sap-fieldglass-odata-analytic-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-fieldglass/refs/heads/main/authentication/sap-fieldglass-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Contingent Workforce
- External Talent
- Human Capital Management
- Services Procurement
- Statements of Work
- Vendor Management
- Workforce Management
---
