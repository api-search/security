---
api_key_in: []
api_specs:
- filename: ostrom-openapi-original.json
  format: json
  label: Ostrom API
  slug: ostrom-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/openapi/ostrom-openapi-original.json
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Ostrom Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Ostrom secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Ostrom
provider_slug: ostrom
scheme_count: 2
schemes:
- description: A `ClientAccessToken` is obtained via the [OAuth 2.0 Client Credentials grant](https://www.oauth.com/oauth2-servers/access-tokens/client-credentials/) and carries authorization to access all functionalities and data in your Ostrom account. Full details at [The ClientAccessToken](/api/reference#getting-an-access-token)
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://auth.sandbox.ostrom-api.io/oauth2/token
  name: ClientAccessToken
  sources:
  - openapi/ostrom-openapi-original.json
  type: oauth2
- name: OAuth2BasicAuth
  scheme: basic
  sources:
  - openapi/ostrom-openapi-original.json
  type: http
slug: ostrom-authentication
source_filename: ostrom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: openapi/ostrom-openapi-original.json\ndocs: https://docs.ostrom-api.io/reference/authentication\nnotes: >-\n  OAuth2 client-credentials grant. Client registers in the Developer Portal\n  (https://developer.ostrom-api.io/) to obtain a client_id/client_secret per\n  environment. Token request uses HTTP Basic auth (base64 client_id:client_secret)\n  with grant_type=client_credentials against the environment token endpoint\n  (auth.sandbox / auth.production). The returned access_token (Bearer, expires_in\n  ~3599s) authorizes calls. Roles USER (own data) and PARTNER (multi-user with consent).\ntoken_endpoints:\n  sandbox: https://auth.sandbox.ostrom-api.io/oauth2/token\n  production: https://auth.production.ostrom-api.io/oauth2/token\nroles:\n- USER\n- PARTNER\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: ClientAccessToken\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: https://auth.sandbox.ostrom-api.io/oauth2/token\n    scopes: 0\n  description: A `ClientAccessToken` is obtained via the [OAuth 2.0 Client Credentials grant](https://www.oauth.com/oauth2-servers/access-tokens/client-credentials/)\n    and carries authorization to access all functionalities and data in your Ostrom account.\n    Full details at [The ClientAccessToken](/api/reference#getting-an-access-token)\n  sources:\n  - openapi/ostrom-openapi-original.json\n- name: OAuth2BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/ostrom-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ostrom/refs/heads/main/authentication/ostrom-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Company
- Energy
- Electricity
- Green Energy
- Smart Meter
- Dynamic Pricing
- Germany
- Sustainability
- Webhooks
- API
---
