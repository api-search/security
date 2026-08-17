---
api_key_in:
- header
api_specs:
- filename: responsys-openapi.yml
  format: yaml
  label: Oracle Responsys REST API
  slug: oracle-responsys-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/responsys/refs/heads/main/openapi/responsys-openapi.yml
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
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.oracle.com/en/cloud/saas/marketing/responsys-develop/API/GetStarted/Authentication/auth-endpoints-rest.htm\ndocs: https://docs.oracle.com/en/cloud/saas/marketing/responsys-develop/API/GetStarted/Authentication/auth-endpoints-rest.htm\nspec_gap: >-\n  The harvested Swagger 2.0 (openapi/_original/responsys-openapi.json) declares NO\n  securityDefinitions and applies no security to any of its 88 operations, so the machine\n  contract reads as an unauthenticated API. It is not. Everything below was read from the\n  documentation, not derived from the spec.\nsummary:\n  types: [token]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Responsys REST API uses a two-step token flow: authenticate against the\n    auth/token endpoint to obtain a short-lived authToken and the pod endPoint,\n    then pass the token on subsequent requests in the Authorization header.\nschemes:\n- name: ResponsysAuthToken\n  type:\
  \ apiKey\n  in: header\n  parameter: Authorization\n  description: >-\n    Session auth token obtained from POST /rest/api/v1.3/auth/token and sent in\n    the Authorization header on every subsequent REST call. Tokens are short-lived\n    and can be refreshed via the auth/token endpoint.\n  token_endpoint: /rest/api/v1.3/auth/token\n  auth_types:\n  - password        # user_name + password\n  - token           # refresh an existing authToken\n  - certificate     # server-side certificate (OAuth-like signed assertion)\n  sources: [docs]\nlogin_hosts:\n- url: https://login2.responsys.net\n  note: Responsys Interact 2 authentication host.\n- url: https://login5.responsys.net\n  note: Responsys Interact 5 authentication host.\n- url: https://login.rsys8.net\n  note: Responsys Interact 8 authentication host.\n- url: https://login.rsys9.net\n  note: Responsys Interact 9 authentication host.\n- pattern: https://{AccountToken}-api.responsys.ocs.oraclecloud.com\n  note: >-\n    Global Routing\
  \ REST endpoint. The account's value is shown in the Responsys UI under\n    Account > Global settings > Account configuration, in the WS End Point field.\n- pattern: \"{AccountToken}-aftm.responsys.ocs.oraclecloud.com\"\n  note: Global Routing endpoint for the AFTM / asynchronous API.\nendpoint_discovery:\n  required: true\n  note: >-\n    Two hops by design. Authenticate against a login host, then use the endPoint URL\n    returned in the auth response as the base URL for every subsequent call. Continuing to\n    call the login host after authenticating is the most common integration error.\nnetwork_reachability:\n  publicly_reachable: false\n  probed: '2026-08-13'\n  note: >-\n    TCP connect to port 443 on login5.responsys.net (162.223.232.188) and\n    login2.responsys.net times out from the public internet, so the auth endpoint cannot\n    be exercised — even anonymously — from an unprovisioned network. DNS resolves fine\n    (login5 -> oapi5.responsys.net). This is an access posture,\
  \ not an outage.\n"
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
- Push Notifications
- SMS
- Webhooks
- Oracle
- Martech
---
