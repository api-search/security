---
api_key_in:
- header
api_specs:
- filename: bluecore-openapi.yml
  format: yaml
  label: Bluecore API
  slug: bluecore-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/openapi/bluecore-openapi.yml
auth_types:
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Bluecore Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Bluecore secures its APIs with oauth2 and http-bearer across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Bluecore
provider_slug: bluecore
scheme_count: 1
schemes:
- description: Bearer access token obtained from the client-credentials token endpoint. Value is "Bearer " followed by the token returned by POST https://auth.bluecore.com/oauth/token.
  in: header
  name: GlooAuth
  parameter: authorization
  scheme: bearer
  sources:
  - openapi/bluecore-openapi.yml
  - https://developers.bluecore.com/reference/authn_getaccesstoken
  type: http
slug: bluecore-authentication
source_filename: bluecore-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.bluecore.com/reference/authn\ndocs: https://developers.bluecore.com/reference/authn\nsummary:\n  model: oauth2-client-credentials\n  types:\n  - oauth2\n  - http-bearer\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Bluecore uses the standard OAuth 2.0 client-credentials grant. Clients POST client_id +\n    client_secret to https://auth.bluecore.com/oauth/token (audience https://a.bluecore.com,\n    grant_type client_credentials) and receive a Bearer access_token valid for 24 hours (86,400s).\n    Requests to the API then send `authorization: Bearer <token>`. In the published per-operation\n    OpenAPI the bearer scheme is modelled as an apiKey security scheme named \"GlooAuth\"\n    (in: header, name: authorization) rather than an oauth2 scheme, so the mechanical oauth2\n    scope derivation does not fire; the real flow and scopes are captured here and in scopes/.\n\
  schemes:\n- name: GlooAuth\n  type: http\n  scheme: bearer\n  in: header\n  parameter: authorization\n  description: >-\n    Bearer access token obtained from the client-credentials token endpoint. Value is\n    \"Bearer \" followed by the token returned by POST https://auth.bluecore.com/oauth/token.\n  sources:\n  - openapi/bluecore-openapi.yml\n  - https://developers.bluecore.com/reference/authn_getaccesstoken\ntoken_endpoint:\n  url: https://auth.bluecore.com/oauth/token\n  grant_type: client_credentials\n  audience: https://a.bluecore.com\n  token_type: Bearer\n  expires_in: 86400\n  credentials_docs: https://help.bluecore.com/help/create-an-api-key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluecore/refs/heads/main/authentication/bluecore-authentication.yml
summary_line: oauth2/http-bearer · 1 scheme
tags:
- Company
- Retail
- Marketing
- Customer Data Platform
- Personalization
- Email
- SMS
- Messaging
- eCommerce
- Consent
---
