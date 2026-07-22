---
api_key_in: []
api_specs:
- filename: yokoy-openapi-original.json
  format: json
  label: Yokoy API
  slug: yokoy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yokoy/refs/heads/main/openapi/yokoy-openapi-original.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Yokoy Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Yokoy secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Yokoy
provider_slug: yokoy
scheme_count: 1
schemes:
- description: 'Authentication to the Yokoy API relies on the standard OAuth2 client credentials flow.


    **1. Obtain an access token**


    Perform a `POST` request to

    `https://accounts.yokoy.ai/oauth2/token`. Pass the client ID

    and client secret as username and password in a basic auth

    header. Set the content-type to

    `application/x-www-form-urlencoded` and specify

    `grant_type=client_credentials` in the body.


    > Note:'
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://accounts[.test].yokoy.ai/oauth2/token
  name: OAuth2
  sources:
  - openapi/yokoy-openapi-original.json
  type: oauth2
slug: yokoy-authentication
source_filename: yokoy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/yokoy-openapi-original.json\ndocs: https://developer.yokoy.ai/docs/overview/authentication\ncredentials_docs: https://help.yokoy.ai/en/articles/110470-get-access-credentials-for-yokoy-api\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://accounts[.test].yokoy.ai/oauth2/token\n    scopes: 0\n  description: |-\n    Authentication to the Yokoy API relies on the standard OAuth2 client credentials flow.\n\n    **1. Obtain an access token**\n\n    Perform a `POST` request to\n    `https://accounts.yokoy.ai/oauth2/token`. Pass the client ID\n    and client secret as username and password in a basic auth\n    header. Set the content-type to\n    `application/x-www-form-urlencoded` and specify\n    `grant_type=client_credentials` in the body.\n\n    > Note:\n  sources:\n  - openapi/yokoy-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yokoy/refs/heads/main/authentication/yokoy-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Spend Management
- Expense Management
- Invoice Management
- Finance Automation
- Corporate Cards
- Fintech
- SaaS
---
