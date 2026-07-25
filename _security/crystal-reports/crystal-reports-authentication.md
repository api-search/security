---
api_key_in:
- header
api_specs:
- filename: crystal-reports-authentication-api-openapi.yml
  format: yaml
  label: Crystal Reports Authentication API
  slug: crystal-reports-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-authentication-api-openapi.yml
- filename: crystal-reports-export-api-openapi.yml
  format: yaml
  label: Crystal Reports Export API
  slug: crystal-reports-export-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-export-api-openapi.yml
- filename: crystal-reports-instances-api-openapi.yml
  format: yaml
  label: Crystal Reports Instances API
  slug: crystal-reports-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-instances-api-openapi.yml
- filename: crystal-reports-metadata-api-openapi.yml
  format: yaml
  label: Crystal Reports Metadata API
  slug: crystal-reports-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-metadata-api-openapi.yml
- filename: crystal-reports-odata-api-openapi.yml
  format: yaml
  label: Crystal Reports OData API
  slug: crystal-reports-odata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-odata-api-openapi.yml
- filename: crystal-reports-reports-api-openapi.yml
  format: yaml
  label: Crystal Reports Reports API
  slug: crystal-reports-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-reports-api-openapi.yml
- filename: crystal-reports-repository-api-openapi.yml
  format: yaml
  label: Crystal Reports Repository API
  slug: crystal-reports-repository-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/openapi/crystal-reports-repository-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Crystal Reports Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crystal Reports secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Crystal Reports
provider_slug: crystal-reports
scheme_count: 2
schemes:
- description: SAP logon token obtained from the /logon/long endpoint. The token value must be enclosed in double quotes when sent in the header.
  in: header
  name: sapLogonToken
  parameter: X-SAP-LogonToken
  sources:
  - openapi/crystal-reports-rest-api.yaml
  type: apiKey
- description: HTTP Basic authentication as an alternative to token-based auth
  name: basicAuth
  scheme: basic
  sources:
  - openapi/crystal-reports-rest-api.yaml
  type: http
slug: crystal-reports-authentication
source_filename: crystal-reports-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crystal-reports-rest-api.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: sapLogonToken\n  type: apiKey\n  in: header\n  parameter: X-SAP-LogonToken\n  description: SAP logon token obtained from the /logon/long endpoint. The token value must\n    be enclosed in double quotes when sent in the header.\n  sources:\n  - openapi/crystal-reports-rest-api.yaml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication as an alternative to token-based auth\n  sources:\n  - openapi/crystal-reports-rest-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crystal-reports/refs/heads/main/authentication/crystal-reports-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Business Intelligence
- Crystal Reports
- Data Analytics
- Enterprise Software
- Reporting
- SAP
---
