---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sap Successfactors Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: SAP SuccessFactors secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: SAP SuccessFactors
provider_slug: sap-successfactors
scheme_count: 2
schemes:
- description: OAuth 2.0 SAML bearer assertion flow.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.successfactors.com/oauth/token
  name: oauth2
  sources:
  - openapi/sap-successfactors-openapi.yml
  type: oauth2
- description: HTTP Basic auth with username@companyId and password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/sap-successfactors-openapi.yml
  type: http
slug: sap-successfactors-authentication
source_filename: sap-successfactors-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sap-successfactors-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.successfactors.com/oauth/token\n    scopes: 0\n  description: OAuth 2.0 SAML bearer assertion flow.\n  sources:\n  - openapi/sap-successfactors-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth with username@companyId and password.\n  sources:\n  - openapi/sap-successfactors-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-successfactors/refs/heads/main/authentication/sap-successfactors-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- HCM
- HR
- Human Resources
- Talent Management
- Payroll
- Enterprise
- SAP
---
