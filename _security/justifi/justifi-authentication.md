---
api_key_in:
- header
api_specs:
- filename: justifi-openapi-original.yml
  format: yaml
  label: JustiFi API
  slug: justifi-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/justifi/refs/heads/main/openapi/justifi-openapi-original.yml
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Justifi Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: JustiFi secures its APIs with oauth2 and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: JustiFi
provider_slug: justifi
scheme_count: 3
schemes:
- description: POST your JustiFi client id and client secret to the token endpoint to receive an access token valid for 24 hours. Test keys are prefixed test_ and live keys are prefixed live_; the key you authenticate with selects the test or live account.
  flow: clientCredentials
  name: OAuthClientCredentials
  token_ttl_seconds: 86400
  token_url: https://api.justifi.ai/oauth/token
  type: oauth2
- description: Pass the access token from the client-credentials grant in the Authorization header on all subsequent requests. A 401 Unauthorized response means the token expired and a new one must be requested.
  in: header
  name: BearerToken
  parameter: Authorization
  scheme: bearer
  type: http
- description: Platforms scope a request to one of their sub accounts (merchants) by passing that sub account id in the Sub-Account request header.
  in: header
  name: SubAccountHeader
  parameter: Sub-Account
  type: apiKey
slug: justifi-authentication
source_filename: justifi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.justifi.tech/gettingStarted\ndocs: https://docs.justifi.tech/gettingStarted\nnote: >-\n  The published OpenAPI declares no components.securitySchemes; the authentication\n  model below is captured from the JustiFi getting-started documentation.\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\nschemes:\n  - name: OAuthClientCredentials\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://api.justifi.ai/oauth/token\n    description: >-\n      POST your JustiFi client id and client secret to the token endpoint to\n      receive an access token valid for 24 hours. Test keys are prefixed test_\n      and live keys are prefixed live_; the key you authenticate with selects the\n      test or live account.\n    token_ttl_seconds: 86400\n  - name: BearerToken\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    description:\
  \ >-\n      Pass the access token from the client-credentials grant in the\n      Authorization header on all subsequent requests. A 401 Unauthorized\n      response means the token expired and a new one must be requested.\n  - name: SubAccountHeader\n    type: apiKey\n    in: header\n    parameter: Sub-Account\n    description: >-\n      Platforms scope a request to one of their sub accounts (merchants) by\n      passing that sub account id in the Sub-Account request header.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/justifi/refs/heads/main/authentication/justifi-authentication.yml
summary_line: oauth2/apiKey · 3 schemes
tags:
- Company
- Fintech
- Payments
- Embedded Payments
- Payment Facilitation
- Payouts
- Developers
- API
---
