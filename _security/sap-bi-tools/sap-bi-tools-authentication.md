---
api_key_in:
- header
api_specs:
- filename: overview
  format: yaml
  label: SAP Analytics Cloud API
  slug: sap-analytics-cloud-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/SACOpenAPI/overview
- filename: sap-analytics-cloud-data-export-api-openapi.yml
  format: yaml
  label: SAP Analytics Cloud Data Export API
  slug: sap-analytics-cloud-data-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/openapi/sap-analytics-cloud-data-export-api-openapi.yml
- filename: overview
  format: yaml
  label: SAP HANA Cloud Data Lake Files REST API
  slug: sap-hana-cloud-data-lake-files-rest-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/HanaCloudDataLake/overview
- filename: overview
  format: yaml
  label: SAP Datasphere API
  slug: sap-datasphere-api
  spec_type: OpenAPI
  url: https://api.sap.com/api/Datasphere/overview
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Bi Tools Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: SAP BI Tools secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: SAP BI Tools
provider_slug: sap-bi-tools
scheme_count: 2
schemes:
- description: OAuth 2.0 authentication using SAML bearer assertion or authorization code grant flow.
  flows:
  - authorizationUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/authorize
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token
  name: oauth2
  sources:
  - openapi/sap-analytics-cloud-api-openapi.yml
  - openapi/sap-analytics-cloud-content-network-api-openapi.yml
  - openapi/sap-analytics-cloud-data-export-api-openapi.yml
  type: oauth2
- description: Logon token obtained from the /logon/long endpoint. Must be included in all subsequent API requests.
  in: header
  name: logonToken
  parameter: X-SAP-LogonToken
  sources:
  - openapi/sap-businessobjects-bi-platform-api-openapi.yml
  type: apiKey
slug: sap-bi-tools-authentication
source_filename: sap-bi-tools-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-analytics-cloud-api-openapi.yml, openapi/sap-analytics-cloud-content-network-api-openapi.yml,\n  openapi/sap-analytics-cloud-data-export-api-openapi.yml, openapi/sap-businessobjects-bi-platform-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/authorize\n    tokenUrl: https://{tenant}.authentication.{region}.hana.ondemand.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 authentication using SAML bearer assertion or authorization code grant\n    flow.\n  sources:\n  - openapi/sap-analytics-cloud-api-openapi.yml\n  - openapi/sap-analytics-cloud-content-network-api-openapi.yml\n  - openapi/sap-analytics-cloud-data-export-api-openapi.yml\n- name: logonToken\n  type: apiKey\n\
  \  in: header\n  parameter: X-SAP-LogonToken\n  description: Logon token obtained from the /logon/long endpoint. Must be included in all subsequent\n    API requests.\n  sources:\n  - openapi/sap-businessobjects-bi-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bi-tools/refs/heads/main/authentication/sap-bi-tools-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Analytics
- Business Intelligence
- Data Visualization
- Reporting
- SAP
---
