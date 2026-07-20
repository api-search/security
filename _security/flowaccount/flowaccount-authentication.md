---
api_key_in: []
api_specs:
- filename: flowaccount-openapi-original.json
  format: json
  label: FlowAccount Open API
  slug: flowaccount-open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/openapi/flowaccount-openapi-original.json
auth_types:
- oauth2
- http
description: 'FlowAccount Open API uses OAuth 2.0 client credentials. A registered integration exchanges its client_id + client_secret at the token endpoint ({base}/token) with grant_type=client_credentials and scope=flowaccount-api to obtain a bearer access token, then sends it as `Authorization: Bearer <token>` on every request. Sandbox and Production credentials are issued separately on registration. Evidence: flowaccount/open-api apps/api/flowaccount-webhook (AuthenticationService.ts, env.json) documents grant_type=client_credentials, scope=flowaccount-api, and a tokenPost flow; the OpenAPI declares the resulting bearer scheme.'
kind: authentication
layout: security
method: searched
name: Flowaccount Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: FlowAccount secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: FlowAccount
provider_slug: flowaccount
scheme_count: 2
schemes:
- flow: clientCredentials
  name: oauth2ClientCredentials
  scopes:
  - flowaccount-api
  sources:
  - https://github.com/flowaccount/open-api
  token_endpoint: '{base}/token'
  token_endpoint_note: Base is the environment server, e.g. https://openapi.flowaccount.com/sandbox for sandbox. grant_type=client_credentials, scope=flowaccount-api, content-type application/x-www-form-urlencoded.
  type: oauth2
- bearerFormat: Reference
  description: Bearer access token obtained from the client-credentials token endpoint.
  name: bearer
  scheme: bearer
  sources:
  - openapi/flowaccount-openapi-original.json
  type: http
slug: flowaccount-authentication
source_filename: flowaccount-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/flowaccount-openapi-original.json\ndocs: https://developers.flowaccount.com/\ndescription: >-\n  FlowAccount Open API uses OAuth 2.0 client credentials. A registered integration\n  exchanges its client_id + client_secret at the token endpoint ({base}/token) with\n  grant_type=client_credentials and scope=flowaccount-api to obtain a bearer access\n  token, then sends it as `Authorization: Bearer <token>` on every request. Sandbox\n  and Production credentials are issued separately on registration. Evidence:\n  flowaccount/open-api apps/api/flowaccount-webhook (AuthenticationService.ts, env.json)\n  documents grant_type=client_credentials, scope=flowaccount-api, and a tokenPost flow;\n  the OpenAPI declares the resulting bearer scheme.\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  scopes:\n  - flowaccount-api\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n\
  \  token_endpoint: \"{base}/token\"\n  token_endpoint_note: >-\n    Base is the environment server, e.g. https://openapi.flowaccount.com/sandbox\n    for sandbox. grant_type=client_credentials, scope=flowaccount-api,\n    content-type application/x-www-form-urlencoded.\n  scopes:\n  - flowaccount-api\n  sources:\n  - https://github.com/flowaccount/open-api\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: Reference\n  description: Bearer access token obtained from the client-credentials token endpoint.\n  sources:\n  - openapi/flowaccount-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flowaccount/refs/heads/main/authentication/flowaccount-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Accounting
- Invoicing
- Payroll
- Point of Sale
- SME
- Finance
- Tax
- Thailand
- Bookkeeping
---
