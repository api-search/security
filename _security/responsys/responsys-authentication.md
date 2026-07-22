---
api_key_in:
- header
auth_types:
- token
description: ''
kind: authentication
layout: security
method: searched
name: Responsys Authentication
name_suffix: Authentication
oauth_flows: []
overview: Responsys secures its APIs with token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Responsys
provider_slug: responsys
scheme_count: 1
schemes:
- auth_types:
  - password
  - token
  - certificate
  description: Session auth token obtained from POST /rest/api/v1.3/auth/token and sent in the Authorization header on every subsequent REST call. Tokens are short-lived and can be refreshed via the auth/token endpoint.
  in: header
  name: ResponsysAuthToken
  parameter: Authorization
  sources:
  - docs
  token_endpoint: /rest/api/v1.3/auth/token
  type: apiKey
slug: responsys-authentication
source_filename: responsys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.oracle.com/en/cloud/saas/marketing/responsys-rest-api/index.html\ndocs: https://docs.oracle.com/en/cloud/saas/marketing/responsys-rest-api/Authentication.html\nsummary:\n  types: [token]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Responsys REST API uses a two-step token flow: authenticate against the\n    auth/token endpoint to obtain a short-lived authToken and the pod endPoint,\n    then pass the token on subsequent requests in the Authorization header.\nschemes:\n- name: ResponsysAuthToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Session auth token obtained from POST /rest/api/v1.3/auth/token and sent in\n    the Authorization header on every subsequent REST call. Tokens are short-lived\n    and can be refreshed via the auth/token endpoint.\n  token_endpoint: /rest/api/v1.3/auth/token\n  auth_types:\n  - password        # user_name + password\n  - token\
  \           # refresh an existing authToken\n  - certificate     # server-side certificate (OAuth-like signed assertion)\n  sources: [docs]\nlogin_hosts:\n- pattern: https://<login>.responsys.net/rest/api/v1.3\n  note: Interactive/login host used to obtain the initial token (e.g. login2/login5.responsys.net).\n- pattern: https://<pod>.responsys.ocs.oraclecloud.com/rest/api/v1.3\n  note: Oracle Cloud pod endpoint returned as endPoint after successful auth; used for data calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/responsys/refs/heads/main/authentication/responsys-authentication.yml
summary_line: token · 1 scheme
tags:
- Company
- Marketing
- Email Marketing
- Marketing Automation
- Campaign Management
- Cross-Channel Marketing
- Customer Engagement
- Oracle
- Martech
---
