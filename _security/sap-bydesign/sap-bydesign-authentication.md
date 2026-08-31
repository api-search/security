---
api_key_in: []
api_specs:
- filename: sap-bydesign-analytics-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Analytics API
  slug: sap-bydesign-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-analytics-api-openapi.yml
- filename: sap-bydesign-crm-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign CRM API
  slug: sap-bydesign-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-crm-api-openapi.yml
- filename: sap-bydesign-financials-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Financials API
  slug: sap-bydesign-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-financials-api-openapi.yml
- filename: sap-bydesign-master-data-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Master Data API
  slug: sap-bydesign-master-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-master-data-api-openapi.yml
- filename: sap-bydesign-procurement-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Procurement API
  slug: sap-bydesign-procurement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-procurement-api-openapi.yml
- filename: sap-bydesign-projects-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Projects API
  slug: sap-bydesign-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-projects-api-openapi.yml
- filename: sap-bydesign-sales-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Sales API
  slug: sap-bydesign-sales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-sales-api-openapi.yml
- filename: sap-bydesign-supply-chain-api-openapi.yml
  format: yaml
  label: SAP Business ByDesign Supply Chain API
  slug: sap-bydesign-supply-chain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bydesign/refs/heads/main/openapi/sap-bydesign-supply-chain-api-openapi.yml
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
