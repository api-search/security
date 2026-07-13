---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Bydesign Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP Business ByDesign secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP Business ByDesign
provider_slug: sap-bydesign
scheme_count: 2
schemes:
- description: HTTP Basic Authentication using SAP Business ByDesign user credentials.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sap-bydesign-odata-api.json
  type: http
- description: OAuth 2.0 authentication for SAP Business ByDesign.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{tenant}.bydesign.cloud.sap/sap/bc/sec/oauth2/token
  name: oAuth2
  sources:
  - openapi/sap-bydesign-odata-api.json
  type: oauth2
slug: sap-bydesign-authentication
source_filename: sap-bydesign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-bydesign-odata-api.json\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic Authentication using SAP Business ByDesign user credentials.\n  sources:\n  - openapi/sap-bydesign-odata-api.json\n- name: oAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.bydesign.cloud.sap/sap/bc/sec/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 authentication for SAP Business ByDesign.\n  sources:\n  - openapi/sap-bydesign-odata-api.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/authentication/sap-bydesign-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- ERP
- Cloud
- Midmarket
- Financials
- CRM
- Procurement
- Supply Chain
- Project Management
- OData
- SOAP
- SAP
---
