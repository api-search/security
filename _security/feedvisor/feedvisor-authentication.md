---
api_key_in: []
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Feedvisor Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Feedvisor secures its APIs with oauth2 and http across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Feedvisor
provider_slug: feedvisor
scheme_count: 2
schemes:
- flow: clientCredentials
  name: OAuth2ClientCredentials
  returns: JSON access_token
  sources:
  - https://github.com/feedvisor/api-sample
  token_request:
    body:
      grant_type: client_credentials
    client_auth: HTTP Basic (base64 of "client_id:client_secret" in Authorization header)
    content_type: application/x-www-form-urlencoded
    method: POST
  token_url: https://api.feedvisor.com/external/oauth/token/
  type: oauth2
- name: BearerToken
  scheme: bearer
  sources:
  - https://github.com/feedvisor/api-sample
  type: http
  usage: 'The access_token from the client-credentials exchange is sent as "Authorization: Bearer <access_token>" on all subsequent External API calls.'
slug: feedvisor-authentication
source_filename: feedvisor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/feedvisor/api-sample\ndocs: https://feedvisor.com\nnotes: >-\n  Grounded in Feedvisor's first-party External API sample code (feedvisor/api-sample,\n  ExternalApiHelper.java / AuthenticationExample.java). The full API reference lives in\n  Feedvisor's gated Knowledge Base; only the auth mechanics observable in the public\n  sample are captured here (no scheme is fabricated).\nsummary:\n  types:\n  - oauth2\n  - http\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.feedvisor.com/external/oauth/token/\n  token_request:\n    method: POST\n    content_type: application/x-www-form-urlencoded\n    body:\n      grant_type: client_credentials\n    client_auth: HTTP Basic (base64 of \"client_id:client_secret\" in Authorization header)\n  returns: JSON access_token\n  sources:\n  - https://github.com/feedvisor/api-sample\n\
  - name: BearerToken\n  type: http\n  scheme: bearer\n  usage: >-\n    The access_token from the client-credentials exchange is sent as\n    \"Authorization: Bearer <access_token>\" on all subsequent External API calls.\n  sources:\n  - https://github.com/feedvisor/api-sample\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/feedvisor/refs/heads/main/authentication/feedvisor-authentication.yml
summary_line: oauth2/http · 2 schemes
tags:
- Company
- Amazon
- E-Commerce
- Retail
- Advertising
- Pricing
- Repricing
- Marketplace
- Machine Learning
- Optimization
---
