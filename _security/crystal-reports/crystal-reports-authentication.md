---
api_key_in:
- header
api_specs:
- filename: openapi.json
  format: json
  label: Crystal Reports REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://api.sap.com/crystal/openapi.json
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
