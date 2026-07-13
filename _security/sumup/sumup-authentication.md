---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: SumUp REST API
  slug: sumup-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/sumup/sumup-openapi/main/openapi.yaml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Sumup Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: SumUp secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: SumUp
provider_slug: sumup
scheme_count: 2
schemes:
- description: API keys allow you easily interact with SumUp APIs. API keys are static tokens. You can create API keys from the [Dashboard](https://me.sumup.com/settings/api-keys)
  name: apiKey
  scheme: Bearer
  sources:
  - openapi/openapi.yaml
  type: http
- description: 'SumUp supports [OAuth 2.0](https://tools.ietf.org/html/rfc6749) authentication for platforms that want to offer their services to SumUp users.


    To integrate via OAuth 2.0 you will need a client credentials that you can create in the [SumUp Dashboard](https://me.sumup.com/settings/oauth2-applications).


    To maintain security of our users, we highly recommend that you use one of the [recommended OAut'
  flows:
  - authorizationUrl: https://api.sumup.com/authorize
    flow: authorizationCode
    scopes: 8
    tokenUrl: https://api.sumup.com/token
  - flow: clientCredentials
    scopes: 8
    tokenUrl: https://api.sumup.com/token
  name: oauth2
  sources:
  - openapi/openapi.yaml
  type: oauth2
slug: sumup-authentication
source_filename: sumup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yaml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: apiKey\n  type: http\n  scheme: Bearer\n  description: API keys allow you easily interact with SumUp APIs. API keys are static tokens.\n    You can create API keys from the [Dashboard](https://me.sumup.com/settings/api-keys)\n  sources:\n  - openapi/openapi.yaml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.sumup.com/authorize\n    tokenUrl: https://api.sumup.com/token\n    scopes: 8\n  - flow: clientCredentials\n    tokenUrl: https://api.sumup.com/token\n    scopes: 8\n  description: |-\n    SumUp supports [OAuth 2.0](https://tools.ietf.org/html/rfc6749) authentication for platforms that want to offer their services to SumUp users.\n\n    To integrate via OAuth 2.0 you will need a client credentials that you can create in\
  \ the [SumUp Dashboard](https://me.sumup.com/settings/oauth2-applications).\n\n    To maintain security of our users, we highly recommend that you use one of the [recommended OAut\n  sources:\n  - openapi/openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sumup/refs/heads/main/authentication/sumup-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Payments
- POS
- Point of Sale
- Card Readers
- Checkout
- Fintech
- Mobile Payments
- Online Payments
---
