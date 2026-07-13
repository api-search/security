---
api_key_in:
- header
api_specs:
- filename: overview
  format: yaml
  label: SAP Analytics Cloud API
  slug: sap-analytics-cloud-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/API_ANALYTICS_CLOUD/overview
- filename: overview
  format: yaml
  label: SAP BusinessObjects BI Platform REST API
  slug: sap-businessobjects-bi-platform-rest-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/BOBJ_BIPLATFORM/overview
- filename: sap-bi-bw4hana-odata-openapi.yml
  format: yaml
  label: SAP BW/4HANA OData API
  slug: sap-bw4hana-odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi/refs/heads/main/openapi/sap-bi-bw4hana-odata-openapi.yml
- filename: overview
  format: yaml
  label: SAP Datasphere API
  slug: sap-datasphere-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/datasphere/overview
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Bi Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP Business Intelligence secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP Business Intelligence
provider_slug: sap-bi
scheme_count: 3
schemes:
- description: OAuth 2.0 authentication for SAP Analytics Cloud
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://{tenant}.sapanalytics.cloud/oauth/token
  name: oauth2
  sources:
  - openapi/sap-bi-analytics-cloud-openapi.yml
  - openapi/sap-bi-datasphere-openapi.yml
  type: oauth2
- description: SAP BusinessObjects logon token obtained from the logon endpoint
  in: header
  name: logonToken
  parameter: X-SAP-LogonToken
  sources:
  - openapi/sap-bi-businessobjects-platform-openapi.yml
  type: apiKey
- description: SAP user credentials for BW/4HANA system
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sap-bi-bw4hana-odata-openapi.yml
  type: http
slug: sap-bi-authentication
source_filename: sap-bi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-bi-analytics-cloud-openapi.yml, openapi/sap-bi-businessobjects-platform-openapi.yml,\n  openapi/sap-bi-bw4hana-odata-openapi.yml, openapi/sap-bi-datasphere-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://{tenant}.sapanalytics.cloud/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authentication for SAP Analytics Cloud\n  sources:\n  - openapi/sap-bi-analytics-cloud-openapi.yml\n  - openapi/sap-bi-datasphere-openapi.yml\n- name: logonToken\n  type: apiKey\n  in: header\n  parameter: X-SAP-LogonToken\n  description: SAP BusinessObjects logon token obtained from the logon endpoint\n  sources:\n  - openapi/sap-bi-businessobjects-platform-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: SAP user credentials\
  \ for BW/4HANA system\n  sources:\n  - openapi/sap-bi-bw4hana-odata-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bi/refs/heads/main/authentication/sap-bi-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
---
