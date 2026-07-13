---
api_key_in: []
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wordline Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Worldline secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Worldline
provider_slug: wordline
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://sbx-wlip.api1-eu2.psapigateway.preprod.giservices.io/token
  name: basic
  sources:
  - openapi/worldline-card-issuing-api-2.41.1.json
  type: oauth2
- description: 'The ''Authorization'' field must be filled with an access token.

    #### How to get an access token

    To request an access token, the Initiating Party must digitally sign the relevant request headers using the private key that corresponds to the certificate uploaded to the Open Banking Service Portal. This action is to be performed in the `POST /token` endpoint.


    Upon a successful request, the Open Banki'
  name: Authorization
  scheme: bearer
  sources:
  - openapi/worldline-open-banking-payment-initiation-3.15.0.yaml
  type: http
slug: wordline-authentication
source_filename: wordline-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/worldline-card-issuing-api-2.41.1.json, openapi/worldline-open-banking-payment-initiation-3.15.0.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: basic\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://sbx-wlip.api1-eu2.psapigateway.preprod.giservices.io/token\n    scopes: 0\n  sources:\n  - openapi/worldline-card-issuing-api-2.41.1.json\n- name: Authorization\n  type: http\n  scheme: bearer\n  description: |-\n    The 'Authorization' field must be filled with an access token.\n    #### How to get an access token\n    To request an access token, the Initiating Party must digitally sign the relevant request headers using the private key that corresponds to the certificate uploaded to the Open Banking Service Portal. This action is to be performed in the `POST /token` endpoint.\n\n    Upon a successful request, the Open Banki\n  sources:\n\
  \  - openapi/worldline-open-banking-payment-initiation-3.15.0.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordline/refs/heads/main/authentication/wordline-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Payments
- Payment Processing
- Acquiring
- Issuing
- Open Banking
- Digital Banking
- FinTech
- Europe
---
